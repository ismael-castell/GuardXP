# ASTrack Gateway - Proof of Concept

HTTP/HTTPS tracker blocking based on mitmproxy + ASTrack clean resources

## Setup

1. Create base folder for certificates and geolocation DB:
   ```bash
   mkdir -p ~/.astrack-gw/geoip2_db
   cd ~/.astrack-gw
   wget https://github.com/FyraLabs/geolite2/releases/download/1738783496/GeoLite2-Country.mmdb -P ./geoip2_db
   ```

2. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/demo-guardxp-gateway.git
   cd demo-guardxp-gateway
   ```

3. Start the application:
   ```bash
   docker-compose up --build
   ```

## Prerequisites

- Docker and Docker Compose installed
- Internet connection for downloading the GeoLite2 database

## Notes

- The GeoLite2 database is used for geolocation services
- Certificates are automatically generated in the `.astrack-gw` directory
- For production deployments, additional configuration may be required


