# Container-Structure-Test

Run sudo curl -LO https://github.com/GoogleContainerTools/container-structure-test/releases/latest/download/container-structure-test-linux-amd64 && sudo chmod +x container-structure-test-linux-amd64 && sudo mv container-structure-test-linux-amd64 /usr/local/bin/container-structure-test

sudo container-structure-test test --image mg-backend-web --config test.yml

```
(base) cipl1168@cipl1168ROR:~/Personal-Github/Container-Structure-Test$ sudo container-structure-test test --image mg-backend-web --config test.yml 

=================================
====== Test file: test.yml ======
=================================
=== RUN: Command Test: say hello world
--- PASS
duration: 579.286218ms
stdout: hello
world

=== RUN: File Existence Test: Check if main app file exists
--- FAIL
duration: 0s
Error: Error examining file in container: Error retrieving file from container: API error (404): Could not find the file /var/www/app/app/controllers/application.py in container 4ff83de0994bf48e703926e77f1ba8421eeae3943f7dc9ea126bc997dc9766c0

=================================
============ RESULTS ============
=================================
Passes:      1
Failures:    1
Duration:    579.286218ms
Total tests: 2

FAIL
FATA[0000] FAIL 

```