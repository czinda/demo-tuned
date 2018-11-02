# demo-tuned
Quick demo of tuned capabilities

Tuned provides recommended configurations for common workloads
* Easy to apply
* Easy to customize
* Persists across reboots
* Installed and enabled with RHEL 7
* Available for RHEL 6 as well

Question: ever opened a case or search KBase for best practices related to performance?
* Predefined sysctl and sysfs settings, based on best practices and real-world workloads
* Number of predefined profiles for common use cases such as:
  * Throughput-performance
  * Virtual-guest
  * Network-latency for low latency
  * Additional Profiles for:
    * Atomic and OpenShift
    * Oracle (via optional repo)
    * SAP & SAP HANA included in RHEL for SAP sub

To view the available installed profiles, run:

```# tuned-adm list```

To view the currently activated profile, run:

```# tuned-adm active (also in list cmd)```

To select or activate a profile, run:

```# tuned-adm profile <profile_name>```

To disable all tuning:

```# tuned-adm off```

[Reference Documentation](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/performance_tuning_guide/chap-red_hat_enterprise_linux-performance_tuning_guide-tuned)
