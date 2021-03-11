# Alethio Ethereum Explorer

This repository contains docker-compose file to start [Alethio Ethereum lite explorer](https://github.com/Alethio/ethereum-lite-explorer).

## Usage

- Start

  ```
  ./eth-explorer start
  ```

- Access

  Open http://127.0.0.1:8080 in your browser.

- Stop
  ```
  ./eth-explorer stop
  ```

## Service

You can use a systemd service to start and stop docker containers at system reboot.

- Copy [eth-explorer.service](eth-explorer.service) file to `/etc/systemd/system`
- Enable the service

  ```
  sudo systemctl enable eth-explorer
  ```

- Start the service

  ```
  sudo systemctl start eth-explorer
  ```

- Stop the service

  ```
  sudo systemctl stop eth-explorer
  ```

- Status of the service

  ```
  sudo systemctl status eth-explorer
  ```

## [License](LICENSE)
