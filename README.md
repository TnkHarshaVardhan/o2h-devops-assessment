# o2h DevOps Assessment

DevOps Fresher Assessment Submission

Homepage feature added.


# Task 5: Troubleshooting Scenarios

## Scenario 1: Docker Container Exits Immediately After Startup

### Possible Reasons

1. Application crashes due to code errors.
2. Incorrect CMD or ENTRYPOINT in Dockerfile.
3. Required dependencies are missing.
4. Port conflicts.
5. Environment variables are missing.

### How to Debug

```bash
docker ps -a
docker logs <container_id>
docker inspect <container_id>
```

* Check container status.
* View container logs.
* Inspect container configuration.
* Run container interactively if needed.

---

## Scenario 2: Application Works Locally but Not on Server

### What Will You Check?

1. Server firewall settings.
2. Port accessibility.
3. Environment variables.
4. Application logs.
5. Network connectivity.
6. Docker container status.

### How Will You Identify the Issue?

```bash
ping <server-ip>
curl localhost:3000
netstat -tulnp
docker logs <container_id>
```

* Verify connectivity.
* Check whether the application port is open.
* Review application and container logs.
* Confirm services are running correctly.
