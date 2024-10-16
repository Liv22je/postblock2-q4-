def mapper(key, value):
"""
Our user-defined mapper function.
:param key: Document identifier (e.g., hostname).
:param value: Content of the document.
"""
for term in cleaner(value):
yield (key, (term, 1))
