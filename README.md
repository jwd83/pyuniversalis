# pyuniversalis
A simple python class to access the FFXIV marketboard API Universalis. Only works by region at the moment and defaults to `North-America`

Presently requires a folder at `./log/` relative to itself to store JSON responses.

Example code:

```python
from pyuniversalis import Universalis

u = Universalis()

items = u.get_marketable_items()

print(f"Found {len(items)} marketable items.")

u.get_item_current_data_by_region(39872)

u.get_item_sale_history_by_region(item)


```

