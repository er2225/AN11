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
