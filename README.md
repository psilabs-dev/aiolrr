# aiolrr
Asynchronous LANraragi API client.

```python
import asyncio
from aiolrr import LRRClient

lrr_host = "http://localhost:3000"
lrr_api_key = "your-api-key"
lrr = LRRClient(lrr_host, lrr_api_key=lrr_api_key)

archive_id = "your-archive-id"
metadata = asyncio.run(lrr.get_archive_metadata(archive_id))
print(metadata)
```