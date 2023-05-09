# Why?

## Data over the wire

Select only fields you want

<div class="notes">
odata has had this for a long time but odata is very slow and relies on the url which has a max length
</div>

## Amount of requests

Aggregate requests into 1

Does HTTP2 solve this?

## Why not?

- N+1 queries
- Caching gets tricky

<div class="notes">
Caching gets handled by clients/servers like Apollo instead of the Browser
</div>
