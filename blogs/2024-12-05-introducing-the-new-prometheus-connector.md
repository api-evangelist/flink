---
title: "Introducing the new Prometheus connector"
url: "https://flink.apache.org/2024/12/05/introducing-the-new-prometheus-connector/"
date: "Thu, 05 Dec 2024 18:00:00 +0000"
author: ""
feed_url: "https://flink.apache.org/posts/index.xml"
---
We are excited to announce a new sink connector that enables writing data to Prometheus (FLIP-312). This articles introduces the main features of the connector, and the reasoning behind design decisions. This connector allows writing data to Prometheus using the Remote-Write push interface, which lets you write time-series data to Prometheus at scale.
