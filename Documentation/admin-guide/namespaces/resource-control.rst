===========================
Namespaces research control
===========================

* There are a LOT of kinds of objects | kernel /
  * do NOT have individual limits OR
  * have limits / ineffective | set of processes -- is allowed to -- switch user ids
* if user namespaces enabled | kernel / people NOT trust their users OR their users programs to play -> problems become more acute
* memory control groups are enabled | kernels / enable user namespaces
* recommendations
  * userspace -- configure -- memory control groups / limit how much memory user's can use
    * way to configure memory control groups
      * installing the `libcgroup` package / present | most distros
        * edit /etc/cgrules.conf, /etc/cgconfig.conf
        * set up libpam-cgroup
