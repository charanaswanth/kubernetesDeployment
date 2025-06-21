1. Create persistentVolume and persistentVolumeClaim
2. Create psql deployment and service
3. Service is created as NodeType to connect from outside the minikube cluster
4. Validate psql DB connectivity
    - Get minikube IP - minikube ip
    - Get NodePort - kubectl get svc
    - From the host run a docker container in iterative mode - docker run -it --rm postgres:latest bash
        - psql -h <minikubeIP> -p <nodePort> -U <DB_USERNAME> -d <DB_NAME>
        - provide DB_PASSWORD on prompt