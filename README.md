# Tribler-tester
Run flake8 on all Trilber repos
Output: https://travis-ci.com/cclauss/Tribler-tester

* $ __$ flake8 . --count --select=E901,E999,F821,F822,F823 --show-source --statistics__

__E901,E999,F821,F822,F823__ are the "_showstopper_" [flake8](http://flake8.pycqa.org) issues that can halt the runtime with a SyntaxError, NameError, etc. Most other flake8 issues are merely "style violations" -- useful for readability but they do not effect runtime safety.
* F821: undefined name `name`
* F822: undefined name `name` in `__all__`
* F823: local variable name referenced before assignment
* E901: SyntaxError or IndentationError
* E999: SyntaxError -- failed to compile a file into an Abstract Syntax Tree

Key: ❌ ✅ --> Tests are failing on Python 2 but passing on Python 3

| Repo | 10 Dec 2018 |
| --- | --- |
| PlebNet | ✅ ❌ | 
| application-tester | ✅ ❌ |
| cloudomate | ✅ ✅ |
| decentral-market | ✅ ❌ |
| decentralized-mortgage-market | ✅ ❌ |
| deployment-scripts | ✅ ❌ |
| dispersy | ❌ ❌ |
| fake-tribler-api | ✅ ❌ |
| gumby | ✅ ❌ |
| py-ipv8 | ✅ ❌ |
| pymdht | ❌ ❌ |
| tribler | ❌ ❌ |
| ipv8-android-app | not working |

# Deep dive on Tribler/tribler
Repo-specific tests are being run at: https://github.com/cclauss/Tribler-tribler-tester

| Directory | 10 Dec 2018 |
| --- | --- |
| . | ❌ ❌ | 
| .sonar | ✅ ❌ | 
| tribler/Tribler | ✅ ❌ |
| tribler/Tribler/Core | ✅ ❌ |
| tribler/Tribler/Main | ✅ ❌ |
| tribler/Tribler/Test | ✅ ❌ |
| tribler/Tribler/community | ✅ ❌ |
| tribler/TriblerGUI | ❌ ❌ |
| tribler/TriblerGUI/dialogs | ✅ ❌ |
| tribler/TriblerGUI/widgets | ✅ ❌ |
| tribler/debian | ✅ ✅ |
| tribler/twisted/plugins | ✅ ✅ |
| tribler/win | ✅ ✅ |

