# Prerequisites

- Python
- Django

# Guide 

## 1. Clone the repository:

- git clone https://github.com/GaneshNair05/Project-vendor.git
- cd "project-name"

## 2.Create a virtual environment:
- python -m venv env
- cd env\scripts
- activate

## 3.Install dependencies:
- pip install -r requirements.txt 

## 4.Database setup:
- python manage.py migrate

## 5.Start the server:
- python manage.py runserver  

# API Endpoints
## Vendor API  
● POST /api/vendors/: Create a new vendor.  
● GET /api/vendors/: List all vendors.  
● GET /api/vendors/{vendor_id}/: Retrieve a specific vendor's details.  
● PUT /api/vendors/{vendor_id}/: Update a vendor's details.  
● DELETE /api/vendors/{vendor_id}/: Delete a vendor  
  
● Vendor Performance Endpoint (GET /api/vendors/{vendor_id}/performance)  
  
## Purchase Order API  
● POST /api/purchase_orders/: Create a purchase order.  
● GET /api/purchase_orders/: List all purchase orders with an option to filter by vendor.  
● GET /api/purchase_orders/{po_id}/: Retrieve details of a specific purchase order.  
● PUT /api/purchase_orders/{po_id}/: Update a purchase order.  
● DELETE /api/purchase_orders/{po_id}/: Delete a purchase order  
  
## Vendor Performance Evaluation  
● GET /api/vendors/{vendor_id}/performance: Retrieve a vendor's performance metrics  

## Historical Performance API  
GET /vendor/historical_performance: List historical performance for all vendors.  
GET /vendor/historical_performance/{id}/: Retrieve historical performance for a specific vendor.  
  
## Update Acknowledgment Endpoint:  
● While not explicitly detailed in the previous sections, consider an endpoint like  
POST /api/purchase_orders/{po_id}/acknowledge for vendors to acknowledge POs.  
● This endpoint will update acknowledgment_date and trigger the recalculationof average_response_time 
