\# Wazuh SOC Home Lab – Windows Security Monitoring \& Incident Detection



\## Overview



This project is a hands-on Security Operations Center (SOC) home lab built using Wazuh, Docker, Windows, and Sysmon.



The goal was to simulate a real SOC monitoring environment where Windows security telemetry is collected, analyzed, mapped to MITRE ATT\&CK techniques, and investigated as security alerts.



\## Architecture



```text

&#x20;                   Windows Endpoint

&#x20;                 Windows 11 Pro

&#x20;                       |

&#x20;                       | Sysmon Events

&#x20;                       |

&#x20;                       v

&#x20;                Wazuh Agent

&#x20;             Windows-SOC-Endpoint

&#x20;                    Agent 003

&#x20;                       |

&#x20;                       | TCP 1514

&#x20;                       v

&#x20;                Wazuh Manager

&#x20;                       |

&#x20;             +---------+---------+

&#x20;             |                   |

&#x20;             v                   v

&#x20;       Wazuh Indexer       Wazuh Analysis

&#x20;             |

&#x20;             v

&#x20;       Wazuh Dashboard

&#x20;             |

&#x20;             v

&#x20;       SOC Investigation

