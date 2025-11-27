# FORKED Sock Shop Microservices Demo

## About This Fork

This is a fork of the original [Sock Shop microservices demo](https://github.com/microservices-demo/microservices-demo) with added **Swagger UI** for API documentation and testing.

### ✨ What's New in This Fork

- **Swagger UI Integration** - Interactive API documentation for all microservices
- **Complete OpenAPI Specifications** - API specs for Catalogue, Carts, Users, Orders, Payment, and Shipping services
- **Easy API Testing** - Test all endpoints directly from the browser

---

## 🚀 Quick Start

### Prerequisites
- Docker Desktop installed
- Docker Compose v2+

### Run the Application

1. **Clone this repository:**
   ```bash
   git clone https://github.com/YOUR-USERNAME/microservices-demo.git
   cd microservices-demo
   ```

2. **Start all services:**
   ```bash
   cd deploy/docker-compose
   docker compose up -d
   ```

3. **Access the application:**
   - **Sock Shop Website**: http://localhost
   - **Swagger UI (API Documentation)**: http://localhost:8081

### Swagger UI

The Swagger UI provides interactive API documentation for all microservices. You can:
- Browse all available API endpoints
- View request/response schemas
- Test API calls directly from the browser
- See example payloads

**Available APIs:**
- **Catalogue** - Product catalog management
- **Carts** - Shopping cart operations
- **Users** - User authentication and management
- **Orders** - Order processing
- **Payment** - Payment authorization
- **Shipping** - Shipping and delivery

---

## 📖 Original Project Information

The Sock Shop application is a user-facing part of an online shop that sells socks. It demonstrates microservice and cloud native technologies.

**Built with:**
- [Spring Boot](http://projects.spring.io/spring-boot/)
- [Go kit](http://gokit.io)
- [Node.js](https://nodejs.org/)
- Docker containers

### Architecture

You can read more about the [application design](./internal-docs/design.md).

### Screenshot

![Sock Shop frontend](https://github.com/microservices-demo/microservices-demo.github.io/raw/master/assets/sockshop-frontend.png)

### Visualizing the Application

Use [Weave Scope](http://weave.works/products/weave-scope/) or [Weave Cloud](http://cloud.weave.works/) to visualize the application topology and monitor the running microservices.

![Sock Shop in Weave Scope](https://github.com/microservices-demo/microservices-demo.github.io/raw/master/assets/sockshop-scope.png)

---

## 🛠️ Using for Testing & Development

This setup is ideal for:
- **API Testing** - Use Swagger UI or export OpenAPI specs to Postman
- **Automated Testing** - OpenAPI specs available in `swagger/specs/` directory
- **Learning Microservices** - Explore real-world microservice architecture
- **Testing Tools** - Practice with tools like Postman, Newman, or Dredd

### OpenAPI Specifications Location

All API specifications are available in:
```
swagger/specs/
├── catalogue.json
├── carts.json
├── users.json
├── orders.json
├── payment.json
└── shipping.json
```

You can import these into any API testing tool.

---

## 🐛 Troubleshooting

### Ports Already in Use

If you see port conflicts:
- Port 80 is used by the main application
- Port 8081 is used by Swagger UI
- Port 8080 is used by edge-router

Change ports in `deploy/docker-compose/docker-compose.yml` if needed.

### Platform Warnings (Apple Silicon)

If you see warnings about `linux/amd64` vs `linux/arm64`, this is normal on Apple Silicon Macs. Docker will automatically handle the emulation.

---

## 📦 Deployment Platforms

The [deploy folder](./deploy/) contains scripts and instructions for various platforms.

### Stopping the Application

```bash
cd deploy/docker-compose
docker compose down
```

### Viewing Logs

```bash
docker compose logs -f [service-name]
# Example: docker compose logs -f catalogue
```

---

## 🤝 Contributing

This is a fork for educational and testing purposes. For contributions to the original project, see the [original repository](https://github.com/microservices-demo/microservices-demo).

For issues related to the Swagger UI integration in this fork, please open an issue in this repository.

---

## 📄 License

Same as the original project - see [LICENSE](LICENSE)

---

## 🔗 Related Resources

- [Original Sock Shop Repository](https://github.com/microservices-demo/microservices-demo)
- [Swagger UI Documentation](https://swagger.io/tools/swagger-ui/)
- [OpenAPI Specification](https://swagger.io/specification/)

---

## ⚠️ Note

The original Sock Shop project is **DEPRECATED** but remains an excellent learning resource for microservices architecture and testing.
