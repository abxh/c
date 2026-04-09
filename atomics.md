# atomics

Concurrency is hard. I have already followed along [this](www.youtube.com/watch?v=d9s_d28yJq0&list=PLfqABt5AS4FmuQf70psXrsMLEDQXNkLq2)
excellent playlist by CodeVault, and have a decent idea of what is there to entail with `pthreads` and "blocking" operations.

However, lockless data structures and atomics have remained a mystery to me, since I was not familiar with terminology and
have not matured with reasoning with concurrency.

Have a look at the different memory ordering that exist in C++ [here](https://en.cppreference.com/w/cpp/atomic/memory_order.html):
- memory_order_relaxed
- memory_order_consume
- memory_order_acquire
- memory_order_release
- memory_order_acq_rel
- memory_order_seq_cst

Yikes. And that page is huge and full of unknown terminologies, already telling me this topic is difficult. Perhaps if I were patient,
I could slog through that page and learn it, but you can see why I put off this topic for some time. Many of the C++ talks on this also
seems too advanced for me to follow along, and overall it seems to be a huge rabbit hole.

So, recently, I looked at [reddit](https://www.reddit.com/r/C_Programming/comments/18djay4/where_can_one_learn_about_std_threads_atomic/).
Nice, some introductory resources. Let's begin this arduous climb.

I begin by reading a portion of this [concurrency primer](assets.bitbashing.io/papers/concurrency-primer.pdf)... I will need to set up
the basic c/c++ files with <stdatomic.h>/<atomic> to get my hands dirty. Beej has a C guide to 
[this](https://beej.us/guide/bgc/html/split/chapter-atomics.html), and there are a bunch of helpful resources on the reddit post on the c
programming subreddit. I should also find a related project to do eventually so I don't wander aimlessly, and perhaps this
[project-based-learning-repo](https://github.com/practical-tutorials/project-based-learning) has an interesting idea.

This is a draft in progress.
