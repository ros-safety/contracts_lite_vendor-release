^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package contracts_lite_vendor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.5.0 (2021-02-12)
------------------
* Library update: Add contract types (`#14 <https://github.com/ros-safety/contracts_lite/pull/14>`_)

  * rename contract_types.hpp to operators.hpp
  * edit testing instructions in readme
  * add helper types and tests
  * update documentation
  * add requirements docs
  * remove assertions.hpp and scalar_flicker.hpp; too specific for this library

0.4.1 (2020-10-26)
------------------
* Vendor package update

  * Add install instructions to README (`#8 <https://github.com/ros-safety/contracts_lite_vendor/pull/8>`_)

* Library update

  * Add missing inclue, re-arrange move statement (`#13 <https://github.com/ros-safety/contracts_lite/pull/13>`_)
  * Add note clarifying 'audit' term (`#12 <https://github.com/ros-safety/contracts_lite/pull/12>`_)
  * Add basic requirements (`#10 <https://github.com/ros-safety/contracts_lite/pull/10>`_)
  * Prettier joining of comments (`#9 <https://github.com/ros-safety/contracts_lite/pull/9>`_)
  * Add contact info to README (`#8 <https://github.com/ros-safety/contracts_lite/pull/8>`_)
  * Enforce that audit macros assume ownership of ReturnStatus (`#6 <https://github.com/ros-safety/contracts_lite/pull/6>`_)


0.4.0 (2020-09-21)
------------------
* Library update: (`#5 <https://github.com/ros-safety/contracts_lite/pull/5>`_)

  * Move-optimize comment string handling
  * Make string serializer for contract violation objects static
  * Move-optimize return status object in enforcement macro
  * Add CONTRACT_COMMENT macro and update readme

0.3.3 (2020-09-16)
------------------
* Library update: (`#4 <https://github.com/ros-safety/contracts_lite/pull/4>`_)

  * Make includes more consistent
  * Use the gcc_7x to_string function
* Contributors: Jeffrey Kane Johnson

0.3.2 (2020-09-10)
------------------
* Delete .gitlab-ci.yml (`#3 <https://github.com/ros-safety/contracts_lite_vendor/issues/3>`_)
* point to github repo, bump version
* Add link to original contracts_lite project in readme (`#2 <https://github.com/ros-safety/contracts_lite_vendor/issues/2>`_)
* Contributors: Jeffrey Kane Johnson

0.3.1 (2020-08-29)
------------------
* update to 0.3.1: Replace '+' operator for ReturnStatus types with '&&'; add '||' operator
* Contributors: Jeffrey Kane Johnson

0.2.0 (2020-08-17)
------------------
* update contracts_lite to 0.2.0
* Contributors: Jeffrey Kane Johnson
