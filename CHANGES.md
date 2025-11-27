# Changes from Original Repository

## Added Features

### Swagger UI Integration
- Added Swagger UI container to `docker-compose.yml`
- Configured to run on port 8081
- Provides interactive API documentation for all microservices

### OpenAPI Specifications
Created complete OpenAPI/Swagger specifications for all services:

- **catalogue.json** - Downloaded from original catalogue service repository
- **carts.json** - Downloaded from original carts service repository  
- **orders.json** - Downloaded from original orders service repository
- **payment.json** - Downloaded from original payment service repository
- **users.json** - Custom specification based on user service endpoints
- **shipping.json** - Custom specification based on shipping service endpoints

All specifications are located in `swagger/specs/` directory.

### Documentation
- Updated README.md with Swagger UI usage instructions
- Added quick start guide
- Added troubleshooting section
- Documented API testing workflows

## Modified Files

- `deploy/docker-compose/docker-compose.yml` - Added swagger-ui service
- `README.md` - Complete rewrite with new features
- Created `swagger/specs/` directory with all API specifications

## Purpose

This fork was created to make the Sock Shop demo more useful for:
- API testing practice
- Automated testing development
- Learning microservices architecture
- Testing with modern API tools

## Original Project

This is a fork of [microservices-demo/microservices-demo](https://github.com/microservices-demo/microservices-demo) which is now deprecated but remains a valuable learning resource.
