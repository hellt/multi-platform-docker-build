# multi-platform-docker-build

1. Launch manually the build workflow.
2. Tmate will present you with an ssh login in the logs
3. Connect to the VM via ssh
4. Get a dockerfile
5. Optionally login with `docker login` using a username/repo/password
5. Run

    ```bash
    docker buildx build --platform linux/amd64,linux/arm64 -t some.repo/foo:0.1.1 . --push
    ```
