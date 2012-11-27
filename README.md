MailMan CLI request handling
============================

This is a fork of [list_requests][0] which adds interactive request handling to
the script.

For now the script can only handle the approve and discard actions.

Intended usage is to run this script using sudo on the local machine that runs
the MailMan lists. It must be installed in the `mailman/bin` folder.

Example session:

```
% sudo /usr/lib/mailman/bin/list_requests -l members
1 Members moderator request(s) waiting

Pending posts:
> id 42 : user@example.com on Sun Nov 25 21:57:58 2012 , Subject: Example
Subject , Reason: Post by non-member to a members-only list

Approve (a) or discard (d) message 42? (ad) <a>
Approving 42
%
```


[0]: http://www.msapiro.net/scripts/list_requests

