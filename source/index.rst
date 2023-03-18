A foothold in the cloud
=========================================================

.. image:: _static/images/attack-infra.png
  :alt: Overview

----

The red team performs real-world attacks. For that we have to pretend to be adversaries that do not wish to be detected
no matter what. Redirectors can be used to proxy requests coming from the target back to our attack infrastructure.
A solution with bounce servers is much more elegant and replacing infrastructure components can be done in minutes.
And automating the server set up process like this also helps in exploring current DevOps methodologies to better
understand the underlying technologies.

----

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Redirectors

   docs/redirectors/README.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Bounce servers

   docs/bouncers/README.md
   docs/bouncers/payments.md
   docs/bouncers/major-providers.md
   docs/bouncers/alt-providers.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Frontend

   docs/frontend/README.md
   docs/frontend/nginx.md
   docs/frontend/masquerading.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Backends

   docs/backends/README.md
   docs/backends/c2s.md
   docs/backends/metasploit.md
   docs/backends/silenttrinity.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Automation

   docs/automation/README.md
   docs/automation/containers.md
   docs/automation/terraform.md
   docs/automation/aws.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Attack machines

   docs/attack/README.md
   docs/attack/vpn.md
   docs/attack/location.md
   docs/attack/ephemeral.md
   docs/attack/server.md
   docs/attack/hardware.md
   docs/attack/software.md
