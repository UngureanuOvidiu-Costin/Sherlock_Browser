# Table Downloads
## Important columns:
- target_path
- total_bytes
- danget_type
- hash
- opened
- site_url

```sql
select target_path, total_bytes,
       opened, hash, danger_type from downloads
group by target_path, danger_type;
```

# Table keyword_search_terms
## Important columns
- term
- normalized_term

# Table urls
## Important columns
- url
- title
- hidden
- visit_count
- last_visit_time

```SQL
select * from urls
where hidden != 0;
```

# Table visited_links
## Important columns
- top_level_url
- visit_count

# Table visits:
	This table has the purpose to corelate other tables.
