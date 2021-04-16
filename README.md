# WHAT?! Docker Registry
### Yep, let's run Docker Registry on OpenShift for our external image repository

README tbd - this runs, but a work in progress still - YouTube demo will be done once I get all the features I want to work.

What works:
1. The docker-registry image runs exposing ports 443 & 5000
2. TLS is added via secret.yaml & environment variables
3. Storage is provded by OCS (cephfs)
4. Service exposes the registry on NodePorts (load-balancer required for ha)

Still in progress (no particular order)
1. Auth (oAuth)
2. UI
3. Object Storage (OCS)
4. ?