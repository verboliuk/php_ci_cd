# CI/CD of simple PHP site

Elastic Beanstalk conf:
1. LoadBalancer: On-Demand instances min 1 - max 4
2. Scalling trigger: CPUutilization 80%
3. Rolling updates: Rolling based on helth
