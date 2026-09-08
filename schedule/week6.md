<frontmatter>
  title: "Week 6"
  pageNav: 2
</frontmatter>

<header class="week-header">
  <p class="eyebrow">Week 6 · 14 Sep - 18 Sep</p>
  <h1>Week 6: <span class="placeholder-text">Performance Testing</span></h1>
  <div class="meta-row">
    <span class="meta-chip">Load Testing</span>
    <span class="meta-chip">Stress Testing</span>
    <span class="meta-chip">Spike Testing</span>
  </div>
</header>

<div class="essential-question">
  <strong>Guiding question:</strong>
  <span class="placeholder-text">Will this system still be fast, stable, and standing when real users arrive all at once?</span>
</div>

## Week Overview

Performance testing is a type of non-functional testing that measures a software system's **speed, stability, and scalability** to see how it behaves under both expected and extreme user loads. The main goal is to identify and eliminate performance bottlenecks before the application is released to the public.

## Core Concepts of Performance Testing

Performance testing isn't a single activity but a collection of different test types, each with a specific purpose. It's typically conducted in a controlled environment that mimics the live production server. When running these tests, engineers focus on key metrics such as:

- **Response Time:** How quickly the system responds to a request.
- **Throughput:** The number of requests the system can handle per second.
- **Error Rate:** The percentage of requests that fail under load.

## Key Types of Performance Testing 📊

There are several kinds of performance tests, but three of the most common are:

1. **Load Testing:** This test assesses the application's performance under **normal and expected user loads**. The goal is to ensure the system meets its performance requirements, known as Service Level Agreements (SLAs), during typical day-to-day operations.
2. **Stress Testing:** This test pushes the system **beyond its maximum expected capacity** to find its breaking point. The objective is to see how the system fails and to identify weak spots that could cause a crash under extreme conditions.
3. **Spike Testing:** This test evaluates how the system responds to **sudden, dramatic increases in user traffic**. It's crucial for applications that expect bursty or viral traffic, as it checks if the system can handle the sudden load and recover quickly.

## Example: An E-commerce Website Preparing for a Holiday Sale 🛍️

Imagine an online store getting ready for a massive Black Friday sales event. The team would use performance testing to ensure the site doesn't crash.

- **Load Testing:** First, they would run a **load test** simulating the site's normal peak traffic—say, 10,000 concurrent users—to confirm that product pages load in under 2 seconds and the checkout process is smooth. This establishes a baseline for normal performance.
- **Stress Testing:** Next, they'd conduct a **stress test** to find the website's absolute limit. They would gradually increase the simulated traffic from 10,000 users up to 20,000, 30,000, and beyond, until the site either crashes or response times become unacceptably slow. This might reveal that the database server is the first component to fail, identifying it as a critical weak spot that needs improvement before the sale.
- **Spike Testing:** Finally, to simulate the exact moment the sale begins, they would run a **spike test**. The test would go from a low user count to over 50,000 users in a matter of seconds. The team would watch to see if the site can handle this sudden influx, perhaps slowing down for a moment but recovering quickly without crashing. This ensures the site can withstand the initial rush of eager shoppers.
