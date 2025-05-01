# Scheduler-Study
Design:
Followed along the suggested implementation for the Multilevel Feedback Queue.

Implementation:
As said before, I followed the suggested implementation with the introduction of a priority field.

Benchmarks:

![rrtest](https://github.com/user-attachments/assets/630e3294-6b9f-4f54-bbb3-59b6a4c966cf)

The test programs “add” and “hog” ran without issue for the standard/default round robin schedulers implementation, producing actual output, but “farm” and “schedpong” were running into issues where they ran out of memory upon all tests so it is not possible to benchmark them as they didn’t produce any useful output.



![mlfqtest](https://github.com/user-attachments/assets/98c9d2d3-a31d-4679-8b4f-02c7cb3fd401)

The test programs “add” and “hog” ran without issue again now for the MLFQ scheduler implementation, if I implemented it correctly, producing similar output, but “farm” and “schedpong” were still not working properly due to the memory issue mentioned before. I also attempted to run matmul with this new implementation, but it had an assertion error. From what I could see it seems to have worked slower compared to the standard rr in these cases.
