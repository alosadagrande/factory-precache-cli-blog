# Boosting Red Hat GitOps ZTP at the network edge using factory-precaching-cli tool
## Summary
The factory-precaching-cli tool is a containerized Go binary that is publicly available in the Telco RAN tools container image. In this blog, we want to show how the factory-precaching-cli tool can drastically reduce the OpenShift installation time when using the Red Hat GitOps Zero Touch Provisioning (ZTP) workflow. This statement becomes very significant when dealing with low bandwidth networks either when connecting to a public or disconnected registry.

⚠️ The factory-precaching-cli tool is a Technology Preview feature only.

Looking at the results in the graph, where the x-axis represents network speed in Mbps, we realize how the installation time increases considerably in low bandwidth networks (under 100Mbps). Notice, that using the factory-precaching-cli tool improves the installation time in those environments. It is important to mention that not everything can be precached as today. So, when precaching, the network speed affects the installation time too, but in a minimal way compared with not using precache. 
