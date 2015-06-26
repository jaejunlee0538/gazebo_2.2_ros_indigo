^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package schunk_powercube_chain
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.6.3 (2015-06-17)
------------------
* fix topic names
* replace brics_actuator
* missing dependency
* use new Trigger from std_srvs
* cleanup/replace cob_srvs
* adapt schunk_powercube_chain to new namespaces
* beautify CMakeLists
* Contributors: ipa-fxm

0.6.2 (2014-12-15)
------------------
* add dependencies
* Contributors: ipa-fxm

0.6.1 (2014-09-22)
------------------

0.6.0 (2014-09-18)
------------------

0.5.6 (2014-08-27)
------------------
* catkin_lint'ing
* Contributors: ipa-fxm

0.5.5 (2014-08-26)
------------------
* cleaning up
* New maintainer
* Contributors: ipa-fxm, ipa-nhg

0.5.4 (2014-03-28)
------------------
* Merge branch 'hydro_dev' into hydro_release_candidate
* merge
* added missing dependency
* Contributors: Florian Weisshardt, ipa-fxm

0.5.3 (2014-03-27)
------------------
* install tags
* merge with ipa320
* merge with ipa320
* some catkin_lint
* Contributors: Felix, ipa-fxm

0.5.2 (2014-03-27)
------------------
* add dep to rostest
* Contributors: Florian Weisshardt

0.5.1 (2014-03-20)
------------------
* removed a lot of code related to packages not available in hydro anymore
* add definitions to get rid of some compiler warnings
* fixed linking error of SDH and CAN libraries
* Initial catkinization. Still a linking error in sdh lib.
* Offsets added in PowercubeChain
* merge conficts solved
* Recover function changed (syncmotion deleted)
* untested version that handels offsets inside ROS.
* IMPORTANT changes in init! No offset used anymore. No limits are set to the modules to avoid errors in the PRL-Modules
* Bug in reset during init fixed
* fix compile issue
* fix compile issue on natty
* remove c++0x
* Recover function improved
* remove std=c++0x
* spare includes deleted
* added little comments
* Restsequence in init() changed to avoid problems during 'init all' if there are more chains on one bus.
* changed error on com to debug message
* change to debug message
* -check of return values added in init() -aborting homing because of out of limits limited to only for PW-modules.
* Merge remote branch 'origin-ipa320/master' into automerge
* added effort to joint states message
* communication check for offset writing added
* communication check for setOffsets added.
* Too much output removed. Velocity smoothing reactivated.
* Init procedure improved in the case that 2 chains access the same bus.
* Check of joint position for limits during homing added to avoid fast movement if module is unreferenced.
* merge errors removed
* initalisation of m_position variable with true position from module added
* first draft of diagnostics class
* first draft of diagnostics class
* slightly changes. work in progress.
* Merge remote branch 'origin-ipa320/master' into automerge
* Merge branch 'master' of github.com:ipa-tif/schunk_modular_robotics
* little format changes
* movestep debuggin and adding force_movevel
* remove info output
* Bugfix in moveVel
* ResetAll replaced by resetModule, Diagnositcs output improved, changes in moveVel
* work in progress on limit handling
* Getting out of soft limits improved
* Output for diagnostics improved
* output for diagnostics improved
* selection of module type by encoder added, reading of module type parameter in .yaml removed
* firmware version dependend swichting between moveVelExt and moveStepExt for PRL-Modules
* automatic ModulType check removed, because Encoder Types are not provided. Info output on homing improved.
* improvments on ModuleType investigation
* merge
* Moduletype is read from module, comments added
* Moduletype is read from module
* Fixed stop of all motor on the bus in error case of one. Now only the motors in a kinematic chain are stopped.
* PW-Module homing tested, Rrecovering of only stall modules added, Stop command in global error case added, check for homing flag bevor homing added
* display version number on init added
* Switching of moveVel and moveStep depending on ModuleTypeadded.
* support for homing PRL and PW modules added
* ModuleType added for support of PW and PRL modules
* changed frequency again to avoid CAN bus crashes
* removed debug messages, changed frequency settings
* update stack description
* modified threading in powercube chain, added velocity calculation and fixed moveStep issues
* removed unused files
* add libm5api as source code package
* fill velocities in controller/state message
* fixed position value bug for stable movements
* remove newlines in diagnosticmsgs
* fixed error state bug
* added errorstring to diagnostic messages, has to be tested on real hardware
* added diagnotic topic for initialization states
* modifications for powercubechain to work with tray and torso
* added operation mode interface for general usage of trajectory controller
* fix move step
* using private namespace
* merge to working version of powercube_chain
* using private nodehandle
* moved powercube_chain to schunk repo
* moved to new repo
* Contributors: Alexander Bubeck, Frederik Hegger, abubeck, cob3-5, ipa-cob3-5, ipa-fmw, ipa-fxm, ipa-tif, ipa320, tif
