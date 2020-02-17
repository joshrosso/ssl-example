These steps will put a self-signed SSL certificate in front of your website.

1. Run your target application.

1. Replace `TARGET_HOST` in your local IP address.

    ```
    TARGET_HOST=10.111.223.195
    ```

1. Replace `TARGET_PORT` with your app's port (e.g. 3000).

    ```
    TARGET_PORT=8000
    ```

1. Run the following.

    ```
    sudo docker run -p 9000:9000  --env-file ./config fsouza/docker-ssl-proxy
    ```

1. Call the app host at port `9000`.
