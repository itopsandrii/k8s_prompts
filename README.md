1 Create pod expose port 8000 image ghcr.io/itopsandrii/http_responce:2.0.0
2 Create livenessProbe expose port 8080
3 Create readinessProbe expose port 8000. Image ghcr.io/itopsandrii/http_responce:2.0.0
4 Create a pod with liveness and readiness probe, both exposed for 8080 port. Liveness - /healthy, readiness - /ready. With volumeMounts to /data.