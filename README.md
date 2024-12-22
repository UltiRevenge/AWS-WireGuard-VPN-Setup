# AWS WireGuard VPN Setup

This repository contains resources and instructions to set up a secure and private Virtual Private Network (VPN) using WireGuard on an AWS EC2 instance.

## Features
- **End-to-End Encryption**: Secures all traffic between client and server.
- **Regional Flexibility**: Deploy in different AWS regions for diverse IP geolocation options.
- **Performance**: WireGuard provides lightweight, fast, and secure VPN connectivity.

## Getting Started
1. **Launch an AWS EC2 Instance**:
   - Choose a region and launch an Ubuntu instance.
   - Open necessary ports in the security group (e.g., UDP 51820).

2. **Install WireGuard**:
   - SSH into the EC2 instance and install WireGuard using:
     ```bash
     sudo apt update && sudo apt install wireguard
     ```

3. **Configure the VPN Server**:
   - Use the configuration file provided in `/server/wg0.conf`.

4. **Set Up the Client**:
   - Use the provided client configuration in `/client/wg0-client.conf`.
   - Import the configuration into your WireGuard client application.

5. **Activate the VPN**:
   - On the server:
     ```bash
     sudo wg-quick up wg0
     ```
   - On the client: Activate the configuration.

## Files
- `/server/wg0.conf`: Example server configuration.
- `/client/wg0-client.conf`: Example client configuration.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
# AWS WireGuard VPN Setup

This repository contains resources and instructions to set up a secure and private Virtual Private Network (VPN) using WireGuard on an AWS EC2 instance.

## Features
- **End-to-End Encryption**: Secures all traffic between client and server.
- **Regional Flexibility**: Deploy in different AWS regions for diverse IP geolocation options.
- **Performance**: WireGuard provides lightweight, fast, and secure VPN connectivity.

## Getting Started
1. **Launch an AWS EC2 Instance**:
   - Choose a region and launch an Ubuntu instance.
   - Open necessary ports in the security group (e.g., UDP 51820).

2. **Install WireGuard**:
   - SSH into the EC2 instance and install WireGuard using:
     ```bash
     sudo apt update && sudo apt install wireguard
     ```

3. **Configure the VPN Server**:
   - Use the configuration file provided in `/server/wg0.conf`.

4. **Set Up the Client**:
   - Use the provided client configuration in `/client/wg0-client.conf`.
   - Import the configuration into your WireGuard client application.

5. **Activate the VPN**:
   - On the server:
     ```bash
     sudo wg-quick up wg0
     ```
   - On the client: Activate the configuration.

## Files
- `/server/wg0.conf`: Example server configuration.
- `/client/wg0-client.conf`: Example client configuration.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
