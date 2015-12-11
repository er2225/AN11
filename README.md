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
