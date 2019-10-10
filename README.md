# WhaTLS

What version of TLS and ciphers is your service using? WhaTLS reports on all SSL 
sessions that were captured and exports the data to CSV.

## What is included in the report?

* capture_file - The name of the capture file where the data was pulled.
* client_hello - The full packet details of the Client Hello packet in the TLS handshake for a given session.
* server_hello - The full packet details of the Server Hello packet in the TLS handshake for a given session.
* negotiated_tls_version - What version of SSL/TLS was chosen for a given session.
* negotiated_cipher_suite - What cipher suite was chosen for a given session.


## Installation

1. `git clone https://github.com/clay584/whatls && cd whatls`
2. `pip install -r requirements.txt`

## Usage

1. Take a packet capture and save to file.
2. Run `./whatls.py MyCaptureFile.pcap`.
3. The CSV report will be saved to `MyCaptureFile.csv`.