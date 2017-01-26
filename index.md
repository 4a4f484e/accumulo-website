---
title: Apache Accumulo
skiph1fortitle: true
legal_notice: Apache Accumulo, Accumulo, Apache Hadoop, Apache Thrift, Apache, the Apache feather logo, and the Accumulo project logo are trademarks of the [Apache Software Foundation](https://www.apache.org).
---
<div class="row">
  <div class="col-md-8">
    <div class="jumbotron" style="text-align: center">
      <h3>Apache Accumulo&reg; is a sorted, distributed key/value store that provides robust, scalable data storage and retrieval.</h3>
      <a class="btn btn-success" href="downloads/" role="button"><i class="fa fa-download fa-lg"></i> Download</a>
    </div>
    <div>
      <p id="home-description">Apache Accumulo is based on the design of Google's <a href="https://research.google.com/archive/bigtable.html">BigTable</a> and is powered by <a href="https://hadoop.apache.org">Apache Hadoop</a>, <a href="https://zookeeper.apache.org">Apache Zookeeper</a>, and <a href="https://thrift.apache.org">Apache Thrift</a>.<br><br>Accumulo has several <a href="{{ site.baseurl }}/features/">novel features</a> such as cell-based access control and a server-side programming mechanism that can modify key/value pairs at various points in the data management process.</p>
    </div>
  </div>
  <div class="col-md-4" id="sidebar">
    <div class="row">
      <div class="col-sm-12 panel panel-default">
        <p style="font-size: 24px; margin-bottom: 0px;">Latest News</p>
        {% for post in site.posts limit:site.num_home_posts %}
        <div class="row latest-news-item">
          <div class="col-sm-12" style="margin-bottom: 5px">
           <span style="font-size: 12px; margin-right: 5px;">{{ post.date | date: "%b %Y" }}</span>
           <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
          </div>
        </div>
        {% endfor %}
        <div id="news-archive-link">
         <p>View all posts in the <a href="{{ site.baseurl }}/news">news archive</a></p>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12 panel panel-default">
        {% capture social-include %}{% include social.md %}{% endcapture %}{{ social-include | markdownify }}
      </div>
    </div>
    <a id="apachecon" href="http://www.apache.org/events/current-event.html"><img src="http://www.apache.org/events/current-event-234x60.png"/></a>
    <a id="accumulo-summit-logo" a href="http://accumulosummit.com/"><img alt="Accumulo Summit" class="img-responsive" src="{{ site.baseurl }}/images/accumulo-summit.png"></a>
  </div>
</div>
