UPDATE public.dtd
SET validfrom = created_at::timestamp
WHERE is_feed = true AND feed_state = 0;

SELECT *
FROM public.dtd
WHERE is_feed IS TRUE and feed_state != 500
ORDER BY typename, version;