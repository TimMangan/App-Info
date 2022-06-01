# Capture Filters: Processes

This is the folder for information on setting up application capture filters for Processes.

Some recapture tools allow you to specify process filters, supporting the ability to ignore file/registry activity by these processes.  Some don't.  And App-V does this dynamically so you don't have to worry about it for that packaging.

It is important not only to document the items we typically want cleaned out of repackaging efforts, but to:

* `Entry`: Document what the thing(s) is/are being removed.
* `Explanation`: What is is/Why it isn't needed.
* `Exceptions`: Any special situations where it should not be removed.

The information provided assumes packaging on x64 systems.

| Entry | Explanation | Exceptions |
|----|----|----|

