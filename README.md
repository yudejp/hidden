# hidden
yude.jp on hidden services

## Access
* Tor: [yude3mzscyufx5u3zup72ium7tgecy3bd67p7t6vqhaywvr7e2gqpcqd.onion](yude3mzscyufx5u3zup72ium7tgecy3bd67p7t6vqhaywvr7e2gqpcqd.onion)
* I2P: [yudejp.i2p/?i2paddresshelper=55ivoba6mo3mqlwvw5lqz7lchxqew2kh77kwkn5shefrj2dp3coq.b32.i2p](yudejp.i2p/?i2paddresshelper=55ivoba6mo3mqlwvw5lqz7lchxqew2kh77kwkn5shefrj2dp3coq.b32.i2p)

## Setup
1. Setup I2P, Tor and H2O web server.
2. Clone this repository including submodules.
    ```
    git clone --recursive https://github.com/yudejp/hidden /var/www/hidden
    ```
3. Create symlinks.
    ```
    sudo ln -s /var/lib/i2p/i2p-config/eepsite/docroot /var/www/hidden/html
    ```
4. Copy `h2o.conf`. (Some modifications e.g. running user may be required.)
    ```
    sudo cp -f /var/www/hidden/h2o.conf /etc/h2o/h2o.conf
    ```
5. Reload H2O.
    ```
    sudo systemctl restart h2o
    ```

## License
This repository is provided under the MIT License.
