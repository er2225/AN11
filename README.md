    select * 
    from public.kickstarter
    where date_started>='2015-01-01'
    
    select * 
    from public.kickstarter
    where funded_percent>=100
    
    select *
    from public.kickstarter
    where goal<10000
    
    select distinct project_id
    from public.kickstarter
    where succeeded IS TRUE
    
    select distinct project_id
    from public.kickstarter
    where succeeded='TRUE'

    select distinct url
    from public.kickstarter
    where status='successful'
    
    select *
    from public.kickstarter
    where sub_category='Short Film'
    
    select *
    from public.kickstarter
    where levles IN (6, 7, 8)
    
    select *
    from public.kickstarter
    where sub_category IN ('Short Film', 'Film & Video', 'Fiction')
    
    select *
    from public.kickstarter
    where sub_cateogry LIKE '%Film%'
    
    select *
    from public.kickstarter
    where name LIKE '&quot%'
    
    select *
    from public.kickstarter
    where reward_levels NOT LIKE '%$20%'
    
    select *
    from public.kickstarter
    where sub_cateogry ILIKE '%film%'
    
    select *
    from public.kickstarter
    where name ILIKE '%syria%'
    
    select distinct category, sub-category
    from public.kickstarter
    where (country='U.S.' OR city IN ('London', 'Paris')) AND status='successful'
    
    select *
    from public.kickstarter
    where ((goal<1000 OR status='successful') AND country='U.S.') 
    AND (category ILIKE '%film%' AND date_updated>='2015-10-01')
    
    
    select distinct category, sub_category, status
    from public.kickstarter
    where ((goal<10000 OR (status='failed' AND country IN ('U.S.', 'Ghana', 'Ethiopia'))
    AND (category ILIKE '%film%' AND date_updated>='2015-10-01'))
    OR status='live' OR pledged>100000
    
