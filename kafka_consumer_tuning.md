1. Kafka Consumer Tuning
2. 
The appConfig.spring.kafka section shows a heavy-duty batch processing configuration:

Batch Processing: type: batch indicates the application processes multiple records at once rather than one-by-one.

High Throughput: max.poll.records: 10000 and fetch.min.bytes: 900000 suggest the app is tuned to grab large chunks of data to minimize I/O overhead.

Timeouts: max.poll.interval.ms: 180000 (3 minutes) gives the application enough time to process these large batches before Kafka considers the consumer "dead" and triggers a rebalance.

2. Thread Pool & Performance
The report-config defines how the application handles file writing in parallel:

Concurrency: It uses two distinct thread pools (file-writer and close-report) both set to a fixed size of 20 threads.

Memory Buffering: file-buffer-size is set to 64KB (65,536 bytes) for both reading and writing, which is a standard optimization to reduce disk syscalls.

Paging: nbRecordsPageSize: 500000 suggests it handles very large datasets, potentially keeping half a million records in memory or processing them in massive increments.
