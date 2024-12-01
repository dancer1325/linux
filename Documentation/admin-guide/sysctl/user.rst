=================================
Documentation for /proc/sys/user/
=================================

kernel version 4.9.0

Copyright (c) 2016		Eric Biederman <ebiederm@xmission.com>

------------------------------------------------------------------------------

* goal
    * "/proc/sys/user"'s sysctl files

* "/proc/sys/user"'s sysctl files
    * uses
        * override the default limits on
            * # of namespaces / per-user
            * # other objects / per-user, per user namespace
    * Reason of the existence of these limits: 🧠stop programs /
        * malfunction (creating a ridiculous number of objects) | BEFORE -- becomes a -- system wide problem 🧠
    * previous default limits
        * high enough / NO program -- should run into -- these limits

* creation of per user per user namespace objects -- are charged to the --
    * user | user namespace /
        * created the object &
        * verified / < default per user limit | that user namespace
    * ALL users / created user namespaces /
        * verified / < per user limits | user namespaces of those users

* TODO:

max_cgroup_namespaces
=====================

  The maximum number of cgroup namespaces that any user in the current
  user namespace may create.

max_ipc_namespaces
==================

  The maximum number of ipc namespaces that any user in the current
  user namespace may create.

max_mnt_namespaces
==================

  The maximum number of mount namespaces that any user in the current
  user namespace may create.

max_net_namespaces
==================

  The maximum number of network namespaces that any user in the
  current user namespace may create.

max_pid_namespaces
==================

  The maximum number of pid namespaces that any user in the current
  user namespace may create.

max_time_namespaces
===================

  The maximum number of time namespaces that any user in the current
  user namespace may create.

max_user_namespaces
===================

  The maximum number of user namespaces that any user in the current
  user namespace may create.

max_uts_namespaces
==================

  The maximum number of user namespaces that any user in the current
  user namespace may create.
