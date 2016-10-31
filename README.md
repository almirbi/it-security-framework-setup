# OS X instructions

1. Change the contents of cmake/FindCheck.cmake with the provided file in the repo
2. In the test files that are using check, add this line right above the ```srunner_run_all``` function call.
   ```srunner_set_fork_status(suite_runner, CK_NOFORK);```
   This allows you to debug the code. Example test file is in the repository.
