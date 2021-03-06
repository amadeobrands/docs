---
title: "Add date function calls"
space: "Reference Guide 6"
parent: "Microflow+Expressions"
---


Adding a time unit to a date. In all examples, the first input can be either a new dateTime (depicted in all examples), a variable of type DateTime or an attribute of a domain entity of type DateTime.

## addMilliseconds

Add a number of milliseconds to a date.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of milliseconds to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x milliseconds.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addMilliseconds(dateTime(2007, 1, 1, 1, 1, 1), 1400)
{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 01 01:01:02:400 CET 2007"
{% endhighlight %}

{% endmarkdown %}</div>

## addSeconds

Add a number of seconds to a date.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of seconds to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x seconds.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addSeconds(dateTime(2007, 1, 1, 1, 1, 1), 2)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 01 01:01:03 CET 2007"

{% endhighlight %}

{% endmarkdown %}</div>

## addMinutes

Add a number of minutes to a date.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of minutes to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x minutes.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addMinutes(dateTime(2007, 1, 1, 1, 1, 1), 3)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 01 01:04:01 CET 2007"

{% endhighlight %}

{% endmarkdown %}</div>

## addHours

Add a number of hours to a date.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of hours to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x hours.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addHours(dateTime(2007, 1, 1, 1, 1, 1), 25)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 02 02:01:01 CET 2007"

{% endhighlight %}

{% endmarkdown %}</div>

## addDays[UTC]

Add a number of days to a date. `addDays` uses the server's calendar and `addDaysUTC` uses the UTC calendar.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of days to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x days.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addDays(dateTime(2007, 1, 1, 1, 1, 1), 3)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 04 01:01:01 CET 2007"

{% endhighlight %}

{% endmarkdown %}</div>

## addWeeks[UTC]

Add a number of weeks to a date. `addWeeks` uses the server's calendar and `addWeeksUTC` uses the UTC calendar.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of weeks to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x weeks.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addWeeks(dateTime(2007, 1, 1, 1, 1, 1), 2)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 15 01:01:01 CET 2007"

{% endhighlight %}

{% endmarkdown %}</div>

## addMonths[UTC]

Add a number of months to a date. `addMonths` uses the server's calendar and `addMonthsUTC` uses the UTC calendar.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of months to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x months.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addMonths(dateTime(2007, 1, 1, 1, 1, 1), 13)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Feb 01 01:01:01 CET 2008"

{% endhighlight %}

{% endmarkdown %}</div>

## addYears[UTC]

Add a number of years to a date. `addYears` uses the server's calendar and `addYearsUTC` uses the UTC calendar.

### Input parameters

*   Initial date
    Type: DateTime
*   The amount of years to be added
    Type: Integer

### Output

A result of type DateTime that corresponds to the initial date plus x years.

<div class="alert alert-info">{% markdown %}

{% highlight java %}
addYears(dateTime(2007, 1, 1, 1, 1, 1), 11)

{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Mon Jan 01 01:01:01 CET 2018"

{% endhighlight %}

{% endmarkdown %}</div><div class="alert alert-warning">{% markdown %}

From Mendix release 6.6, It's also possible to pass Long values to different Add date function calls:

{% highlight java %}
addSeconds(dateTime(1970, 1, 1, 0, 0, 0), (long)(2147483647 + 100))
{% endhighlight %}

results in a datetime that corresponds to

{% highlight java %}
"Tue Jan 19 04:15:47 CET 2038"
{% endhighlight %}

{% endmarkdown %}</div>
