# ports

Portfiles for local repository and development
==============================================

## Installation

### Using Git and the bootstrap script

1. Get clone from git repository 
    ```bash
    git clone https://github.com/SeeSpotRun/ports.git ~/ports
    ```


2. Open sources.conf in a text editor
    ```bash
    sudo vi /opt/local/etc/macports/sources.conf
    ```

    Insert a URL pointing to your local repository location before the rsync URL as shown:
    ```
    file:///Users/username/ports
    rsync://rsync.macports.org/release/tarballs/ports.tar [default]
    ```


3. After you create or update your Portfile, use portindex in the local repository's directory to create or update the index of the ports in your local repository.
    ```bash
    cd ~/ports
    portindex
    ```

## Official References

* http://guide.macports.org/#development
