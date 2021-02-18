Things that could be done to improve muld
=========================================

* Pipe all output to log-file instead of stdout, making it work nicer to put
  into a cronjob, daemonizing, or in other ways just "backgrounding" it
* Provide fancy output when not sending everything to log-file or as a
  complementary way when running interactively such that one is not flooded
  with output, a nice status / progress showing what it is currently doing and
  what it is about to do
* Run it in parallel, each mirror-task is can trivially be run in parallel as
  long as there aren't duplicate downstreams, which should probably be checked
  for
* Some fancy checking on the mirror-config, e.g. are there intentionally
  duplicates and stuff like that
