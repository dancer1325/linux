=====================================
The Linux kernel user-space API guide
=====================================

.. _man-pages: https://www.kernel.org/doc/man-pages/

* goal
    * gather links to kernel's user-space API
        * see man-pages_ project
        * see | kernel tree itself

* TODO:

System calls
============

.. toctree::
   :maxdepth: 1

   unshare
   futex2
   ebpf/index
   ioctl/index
   mseal

Security-related interfaces
===========================

.. toctree::
   :maxdepth: 1

   no_new_privs
   seccomp_filter
   landlock
   lsm
   mfd_noexec
   spec_ctrl
   tee

Devices and I/O
===============

.. toctree::
   :maxdepth: 1

   accelerators/ocxl
   dma-buf-alloc-exchange
   gpio/index
   iommufd
   media/index
   dcdbas
   vduse
   isapnp

Everything else
===============

.. toctree::
   :maxdepth: 1

   ELF
   netlink/index
   sysfs-platform_profile
   vduse
   futex2
   perf_ring_buffer

.. only::  subproject and html

   Indices
   =======

   * :ref:`genindex`
