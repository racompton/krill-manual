.. _doc_krill:

Krill 0.9.4
===========

|docsupdated| |discord| |twitter|

.. |docsupdated| image:: https://img.shields.io/github/last-commit/NLnetLabs/krill-manual.svg?label=docs%20updated
            :target: https://github.com/NLnetLabs/krill-manual/commits/main

.. |discord| image:: https://img.shields.io/discord/818584154278199396?label=rpki%20on%20discord&logo=discord
            :target: https://discord.gg/8dvKB5Ykhy

.. |twitter| image:: https://img.shields.io/twitter/follow/krillrpki?style=social
            :target: https://twitter.com/krillrpki/

Krill is a free, open source Resource Public Key Infrastructure (RPKI) daemon,
featuring a Certificate Authority (CA) and publication server, written by `NLnet
Labs <https://nlnetlabs.nl>`_.

You are welcome to ask questions or post comments and ideas on our `RPKI mailing list <https://nlnetlabs.nl/mailman/listinfo/rpki>`_.
If you find a bug in Krill, feel free to create an issue on GitHub. Krill is distributed under the
Mozilla Public License 2.0.

.. Note:: For a quick summary of what's new and changed in the latest version see the `release notes <https://github.com/NLnetLabs/krill/releases/latest>`_.
          If upgrading consult the :ref:`upgrade guide<doc_krill_upgrade>`.

.. figure:: img/krill-ui-welome.png
    :align: center
    :width: 100%
    :alt: Welcome to Krill

------------

**Krill is intended for:**

- **Organisations who hold address space from multiple Regional Internet
  Registries (RIRs). Using Krill, ROAs can be managed seamlessly for all
  resources within one system.**
- **Organisations that need to be able to delegate RPKI to their customers or
  different business units, so that that they can run their own CA and manage
  ROAs themselves.**
- **Organisations who do not wish to rely on the web interface of the hosted
  systems that the RIRs offer, but require RPKI management that is integrated
  with their own systems using a common UI or API.**

------------

Using Krill, you can run your own RPKI Certificate Authority as a child of one
or more parent CAs, usually a Regional Internet Registry (RIR) or National
Internet Registry (NIR). With Krill you can run under multiple parent CAs
seamlessly and transparently. This is especially convenient if your organisation
holds address space in several RIR regions, as it can all be managed as a
single pool.

Krill can also act as a parent for child CAs. This means you can delegate
resources down to children of your own, such as business units, departments,
members or customers, who, in turn, manage ROAs themselves.

Lastly, Krill features a publication server so you can either publish your
certificate and ROAs with a third party, such as your NIR or RIR, or you publish
them yourself. Krill can be managed with a web user interface, from the command
line and through an API.

.. toctree::
   :maxdepth: 2
   :caption: Getting Started
   :name: toc-getting-started

   before-you-start
   architecture
   install-and-run
   get-started

.. toctree::
   :maxdepth: 2
   :caption: Core
   :name: toc-core

   parent-interactions
   manage-roas
   monitoring

.. toctree::
   :maxdepth: 2
   :caption: Advanced
   :name: toc-advanced

   cli
   multi-user
   publication-server
   manage-children
   ca-keyroll
   ca-migrate-repo


.. toctree::
   :maxdepth: 2
   :caption: Reference
   :name: toc-reference

   testbed
   docker
   upgrade
   failure-scenarios

.. history
.. authors
.. license
