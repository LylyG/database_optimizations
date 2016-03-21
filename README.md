# Database Optimizations

The goal here is to take an existing database and make it run more efficiently.

1. Record the size of your database (in bytes). **578MB**<br>
2. Record the size of your development log. **1.48GB**<br>
3. Give at least one method (feel free to Google) for reducing the size of one of these, yet keeping your data intact. **One place to start would be to consider using VACUUM or auto-vacuum.**<br>
4. Do you think that this is smaller, about right, or larger than the size of databases you'll be working with in your career? **I'd say this is about average for a mid-sized database, but the database size varies a lot depending on your clients' needs so it's hard to say what an average would be like throughout a career.**<br>
5. Now let's talk about the "memory" numbers given on the page. What impact have your changes had on memory usage? If you reload a page again and again (with no code changes in between reloads), does memory used stay the same? Have you ever been able to make memory used go down? **Memory went down drastically in three stages: first after adding indices, then associations, and finally, the most change was seen after modifying the controller.**

### Logs
1. Initial seeding: 1854.8 s
Localhost load time: 2712 s when the server timed out.<br>

2. Seeding after adding 3 indices: 2249s
Localhost load time: 21.8s
Memory: 527MB
Number of Hits: 49,387<br>

3. Re-seeding was not needed. Localhost load time: 14.7s
Memory: 473MB<br>

4. Re-seeding was not needed.
Modified the reports controller.
Localhost load time: 0.08s!!
Memory: 69MB   

## Relection

Part one:
This portion should take about 4 hours to seed and re-seed. I think I'll also need a couple of hours to wrap my head around everything that's happening.

**This ended up taking 5 hours to complete.**<br>    

Part two:
Implementing this feature should take another four hours. I think I'll spend quite a bit of time spinning my wheels and conferring with classmates.
