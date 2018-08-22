---
layout: post
title:  A cynical guide to fixing the gender pay gap
date: "2018-08-22 14:00:00"
image: /figure/source/paygap/paygap.png
share-img: http://www.nathancunn.com/figure/source/paygap/paygap.png
---


It's April 5th, the deadline for reporting gender pay gap figures passed last night and your company reported a mean gender pay gap of 23.6%. Already the tabloids are baying for blood and a trending hashtag on Twitter is calling for the boycott of your company's products. As the headlines point out, for every £1 you pay your male staff your female staff on average get 76p.

The mean gender pay gap is the difference between the mean pay across genders expressed as a percentage of mean male pay, the reporting of which was introduced to highlight disparities in upward mobility across the genders. Examining a breakdown of your staff shows no such disparity as women are quite well represented at the upper levels of your company:

<center>

| Position (Salary)     | # Males | # Females |
| -----------           |-----:| -----:  |
| A (£500,000)     | 6     | 5       |
| B (£125,000)       | 8     | 9       |
| C (£60,000) | 30    | 29      |
| D (£20,000)      | 43    | 74      |

</center>

However, this hasn't been reflected in your gender pay gap figures with a mean pay gap of 23.6% and an even more alarming median pay gap of 66.7% (calculated as before, but using the median pay levels instead of the mean).
<center>

|       | Male salary (£) | Female salary (£) | Gap (%) |
| ----  | ---:            | ----:             | ---:    |
|Mean   | 76,551          | 58,504            | 23.6    |
|Median | 60,000          | 20,000            | 66.7    |

</center>

Despite the uproar you feel relaxed; you know you've always been fair in your hiring process. Comically so, in fact. When a position was to be filled you tossed all the applicants' names into a hat and drew one at random. Perhaps, you think, you're just a victim of random variation. While your methods were fair (at least in some sense of the word) by some misfortune you ended up as a statistical outlier. Were you to start all over again your outcome would be much different.

However, before committing to firing all your staff and starting afresh, you decide to examine the impact such a move is likely to have on your gender pay gap figure. You run a simulation: for every position in the company you randomly assign it as having been filled by a male or female with equal probability, effectively the gender occupying each position will be determined by the toss of a coin. And then, in order to get a feel for the random variation of the results, you construct 10,000 such alternate realities, calculating the mean gender pay gap in each case, and then you consider the outcomes had you been more or less favourable towards female candidates:

<div id='paygapplot'></div>


While some deviation is to be expected, the results surprise you. You had expected that a gender pay gap as extreme as yours would be unlikely, a typical threshold being an event with less than a 5% chance of occurring. However, you discover that roughly one in every eight cases (12.4%) had a pay gap worse than your own, with almost one-third (32.7%) having a pay gap greater than 10%. When you consider the frequency of a pay gap against either gender roughly half of all cases exhibited a pay gap greater than 15%. Clearly you're not as much of an outlier as you expected. Furthermore, had you systematically preferred to employ men for all positions such that women only had a 10% success rate, the probability that you observe a pay gap greater than 15% *in favour of women* actually increases slightly from just under 30% to just over 30%.

Knowing you can't rely on reducing your pay gap by starting over, you say goodbye to your simulated staff and consider what changes can be made to your real staff. Maybe you could make some changes at the upper levels; you could promote one of your female employees into the top positions. This turns out to be somewhat successful: promoting a female staff member from position B into the top earning role, A, would decrease your pay gap from 23.5% to just over 19%. The median pay gap, on the other hand, remains unchanged. An improvement, nonetheless, but unlikely to satisfy the angry masses online.

<center>

| Position (Salary)     | # Males | # Females |
| -----------           |-----:| -----:  |
| A (£500,000)     | 6     | 6       |
| B (£125,000)       | 8     | 8       |
| C (£60,000) | 30    | 29      |
| D (£20,000)      | 43    | 74      |

</center>

<center>

|       | Male salary (£) | Female salary (£) | Gap (%) |
| ----  | ---:            | ----:             | ---:    |
|Mean   | 76,551          | 61,709            | 19.4    |
|Median | 60,000          | 20,000            | 66.7    |

</center>


You consider promoting more women, and yet the problem persists. As it turns out, only promoting five more women will be enough to bring your pay gap to a more reasonable 2.6%. The median pay gap, on the other hand, remains unchanged.
<center>

| Position (Salary)     | # Males | # Females |
| -----------           |-----:| -----:  |
| A (£500,000)     | 6     | 10       |
| B (£125,000)       | 8     | 4       |
| C (£60,000) | 30    | 29      |
| D (£20,000)      | 43    | 74      |

</center>

<center>

|       | Male salary (£) | Female salary (£) | Gap (%) |
| ----  | ---:            | ----:             | ---:    |
|Mean   | 76,551          | 74,532            | 2.6     |
|Median | 60,000          | 20,000            | 66.7    |

</center>

While a swathe of promotions for which men aren't eligible may not be ideal for morale you keep this in the 'maybe' pile. Let's not be naive, though, you're a profit-maximising capitalist and promoting such a large number of staff will be costly and difficult; top staff are paid so handsomely due to the relative rarity of their skillsets. Conversely, lower-paid and relatively lower-skilled workers tend to be more readily replaceable. And with that realisation you find your solution and, luckily, it won't cost you a penny. You examine the impact of your plan and discover that it will bring your mean gender pay gap to 0.7% in favour of women and your median pay gap to 0%. Your egalitarian plan? Fire 20 of the lowest paid female workers and replace them all with male workers.

<center>

| Position (Salary)     | # Males | # Females |
| -----------           |-----:| -----:  |
| A (£500,000)     | 6     | 5       |
| B (£125,000)       | 8     | 9       |
| C (£60,000) | 30    | 29      |
| D (£20,000)      | 63    | 54      |

</center>

<center>

|       | Male salary (£) | Female salary (£) | Gap (%) |
| ----  | ---:            | ----:             | ---:    |
|Mean   | 65,981          | 66,443            | -0.7    |
|Median | 20,000          | 20,000            | 0       |

</center>

While this is a simplified, and incredibly cynical, view of the world, the case presented here is not so far-fetched. In the officially reported figures, the very first company you come across, ["Bryanston School", Incorporated](https://gender-pay-gap.service.gov.uk/viewing/employer-details?e=Z7k4NdWWPkmMySu5kzbpYw%21%21), report a mean gender pay gap of 18%, and a median pay gap of 28.2%. Damning figures if you ignore context. The breakdown of their staff into income quartiles shows that women are evenly represented in the upper quartiles with the pay gap seemingly driven by an over-representation of females in the bottom quartile of earners, similar to the hypothetical company I presented above. Although I certainly wouldn't advise it, a strategy such as that outlined above would likely go a long way towards improving their gender pay gap figures, however it's difficult to know the true underlying cause, when the data are as aggregated as they are.

I want to be clear that I'm not arguing against the existence of a gap in pay between genders; it's impossible to argue when [over three-quarters of British businesses reported a gender pay gap in favour of men](https://www.theguardian.com/news/ng-interactive/2018/apr/05/women-are-paid-less-than-men-heres-how-to-fix-it). While the results as a whole may be indicative of a systematic restriction in the upwards mobility of women in our society, I would urge caution when passing judgement on the pay gap figure of a single company as there's little knowledge of what a reasonable level of variation between companies is. Also, as I hope I've demonstrated here:
    * a relatively large pay gap may not reflect a bias against women; even when positions are filled entirely blind to gender it's still likely that a large pay gap will exist
    * a company with a strong bias towards hiring men, may be more likely to have a pay gap figure more strongly in favour of women than a company with no such bias
    * Furthermore, an improvement in the pay gap figure of a firm need not reflect an improvement in conditions for female workers and, indeed, may reflect an objective disimprovement in the situation of the female workforce.

In particular, this disimprovement may be the case for those at the lower end of the scale, and isn't that really where inequality matters most? Coverage of the gender pay gap would suggest otherwise; how often have you heard stories of actresses being paid less than their male counterparts? Without getting into the fairness of this, I find it bizarre that the wealth of the rich and famous would become the cause of people who could only dream of the income of those they're fighting for. How did society go from outrage against the 1% to outrage that the 1% aren't being paid enough? On a similar note, the chief executive of Channel 4, Alex Mahon, was confronted about a gender pay gap of 29 per cent within the company. When asked how she aimed to address this, she promised to bring about parity among the company's top earners---where currently only 34 of the top 100 earners are female she promised to bring this up to 50 in the coming years. While representation of women at the very top levels is, of course, important, we should ask ourselves if further increasing the wealth of 16---presumably already quite wealthy---women is truly the yardstick for equality we had in mind when we decided to undertake this exercise, and how much these changes will benefit the majority.

*Much of this analysis was done in R, while the graphics represent my first foray into D3, so please let me know if they display weirdly on your machine*

<style>
@import url(http://fonts.googleapis.com/css?family=Open+Sans);
@import url(http://fonts.googleapis.com/css?family=Roboto);
.sliderLine{
    stroke-width: 6;
    stroke-linecap: round;
}
.sliderCircle{
    fill: "white"
}
.genText{
    font-family: 'Open Sans';
    font-size: 11pt;
}
.toolTip {
    position: absolute;
    display: none;
    height: auto;
    background: none repeat scroll 0 0 #ACACACCC;
    padding: 14px;
    text-align: left;
    font-family: 'Open Sans', sans-serif;
}


</style>

<script src="//code.jquery.com/jquery.js"></script>
<script type="text/javascript" src="https://d3js.org/d3.v5.min.js"></script>

<script type = "text/javascript">
    // Note: If you're looking through this to help learn D3 note that this is
    // my first attempt at D3 and none of this is likely to be best practice
    // Functions for generating data
    // Fill an array where each of value is repeated each of lens times
function fillArray(value, lens) {
    var arr = [];
    n = lens.reduce(add, 0);
    for (var i = 0; i < n; i++) {
        for(var j = 0; j < lens[i]; j++) {
            arr.push(value[i]);
        }
    }
    return arr;
}
// Need + as a function instead of an operator
function add(a, b) {
    return a + b;
}

// Calculate the paygap for a particular setup
function get_paygap(p, workers, salaries) {
    var nworkers = workers.reduce(add, 0);
    var staffsalary = fillArray(salaries, workers);
    var femalesalary = 0;
    var malesalary = 0;
    var femaleworkers = 0;
    var maleworkers = 0;
    for (var i = 0; i < nworkers; i++) {
        if(Math.random() < p) {
            femalesalary += staffsalary[i];
            femaleworkers += 1;
        } else {
            malesalary += staffsalary[i];
            maleworkers += 1
        }
    };
    // If either gender is unrepresented then give an extreme value
    if (maleworkers == 0 | femaleworkers == 0) {
        out =  1000 * ((- 1) ** (maleworkers == 0));
    } else {
        out = ((malesalary / maleworkers) - (femalesalary / femaleworkers)) / (malesalary / maleworkers) * 100;
    };
    return out;
}

// Replicate the above 'iter' times
function simulateData(p, workers, salaries, nbins) {
    var dataset = Array(nbins).fill(0);
    for (var i = 0; i < iter; i++) {
        var tmp = get_paygap(p, workers, salaries)
        if (tmp > 100) {
            tmp = 100
        } else if (tmp < -150) {
            tmp  = -150
        }
        dataset[i] = tmp;
    };
    var x = d3.scaleLinear().domain([-150, 100]).nice(nbins);
    var histogram = d3.histogram().domain(x.domain()).thresholds(x.ticks(nbins));
    var data = histogram(dataset);
    return data;
}

// Start SVG
// SVG properties
var w = 768;
var h = w / 2;
var margin = [10, 20, 60, 50];
var padding = 2;
var malecol = "#FC7A57";
var femalecol = "#39A9DB";

// Simulation parameters
var nbins = 50;
var iter = 10000; // Approx. 10,000 companies submitted pay gap figs
var p = 0.5;

// Initialise the data
workers = [115, 59, 17, 11];
salaries = [20000, 60000, 125000, 500000];
var dataset = simulateData(p, workers, salaries, nbins);

// Scales for overall plot
// Means we can reference positions on the plot as values in [0, 1]
var x = d3.scaleLinear()
          .domain([0, 1])
          .range([margin[3], w - margin[1]]);
var y = d3.scaleLinear()
          .domain([0, 1])
          .range([h - margin[2], margin[0]]);

// Scales for the main plot
var xScale = d3.scaleLinear()
               .domain([- 150, 105])
               .range([x(0), x(0.75)]);
var yScale = d3.scaleLinear()
               .domain([0, d3.max(dataset, function(d){return d.length / iter * 100}) * 1.05])
               .range([y(0), y(0.95)]);



// Create the SVG plot
var svg_bar = d3.select("#paygapplot")
                .append("svg")
                .attr("width", w)
                .attr("height", h);

// Create axes
var xAxis = d3.axisBottom()
              .scale(xScale);
var yAxis = d3.axisLeft()
              .scale(yScale);
// Create the floating box attached to the bars
var tooltip = d3.select("body").append("div").attr("class", "toolTip");
// Add the main histogram
svg_bar.selectAll(".hist.rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("class", "hist rect")
       .attr("x", function(d) {
           return xScale(d.x0);
       })
       .attr("y", function(d) {
           return yScale(d.length / iter * 100);
       })
       .attr("width", (w * .75) / nbins - padding)
       .attr("height", function(d) {
           return h - margin[2] - yScale(d.length / iter * 100);
       })
       .attr("fill", barColours)
       .on("mousemove", function(d, i) {
           out = 0
           if(i >= 31) {
               for(var j = i; j <= nbins; j++) {
                   out += dataset[j].length / iter * 100;
               }
               tooltipText = Math.round(out * 100) /100 + "% of cases had a gender pay gap ≥ " + (i * 5 - 150) + "% favouring men"
           } else if(i <= 28) {
               for(var j = 0; j <= i; j++) {
                   out += dataset[j].length / iter * 100;
               }
               tooltipText = Math.round(out * 100) /100 + "% of cases had a gender pay gap ≥ " + (145 - i * 5) + "% favouring women"
           } else {
               out = (dataset[29].length + dataset[30].length) / iter * 100
               tooltipText = Math.round(out * 100) /100 + "% of cases had a gender pay gap within ±5%"
           }
           tooltip
           .style("left", (d3.event.pageX + 10) + "px")
           .style("top", (d3.event.pageY - 100) + "px")
           .style("display", "inline-block")
           .html(tooltipText);
       })
       .on("mouseout", function(d){ tooltip.style("display", "none");});

// Function that colours the histogram bars according to x value
function barColours(d, i) {
    if (d.x0 < -5) {
        return femalecol;
    } else if (d.x0 > 0) {
        return malecol;
    } else {
        return "#ACACAC";
    }
}


// Add in the slider for selecting gender
var sliderStart = w * 0.775;
var sliderEnd = w * 0.925;
var maxSalary = 500000;
var maxWorkers = 200;

function sliderDrag() {
    var newX = d3.mouse(this)[0];
    if (newX < sliderStart) {
        newX = sliderStart;
    } else if (newX > sliderEnd) {
        newX = sliderEnd;
    }
    p = (newX - sliderStart) / (sliderEnd - sliderStart) * 100;
    sliderCircle.attr("cx", newX);
    sliderText.text("Female applicants: " + Math.round(p) + "%");
}

function updatePlot() {
    // Could definitely do this better
    var p = (d3.select(".sliderCircle").attr("cx") - sliderStart) / (sliderEnd - sliderStart);
    for(i = 0; i < 4; i++) {
        workers[i] = Math.round(workers2[i].value * maxWorkers)
        salaries[i] = Math.round(salaries2[i].value * maxSalary)
    }
    dataset = simulateData(p, workers, salaries, nbins);
    yScale.domain([0, d3.max(dataset, function(d) {return d.length / iter * 100}) * 1.05]);
    svg_bar.selectAll(".hist.rect")
           .data(dataset)
           .transition()
           .delay(function(d, i) {
               return i * 10
           })
           .attr("y", function(d) {
               return yScale(d.length / iter * 100);
           })
           .attr("height", function(d) {
               return h - margin[2] - yScale(d.length / iter * 100);
           })
           .attr("fill", barColours)
           .attr("x", function(d) {return xScale(d.x0)});
    svg_bar.select(".y.axis").call(yAxis);
}

var drag = d3.drag()
             .on("drag", sliderDrag)
             .on("start", sliderDrag)
             .on("end", updatePlot);

function barDrag() {
      newWidth = d3.mouse(this)[0] - d3.select(this).attr("x");
      if (newWidth > maxWidth) {
          newWidth = maxWidth;
      } else if (newWidth < 0) {
          newWidth = 0;
      }
      d3.select(this)
        .attr("width", newWidth)
        .datum().value = (newWidth / maxWidth);

     workerLabs.attr("x", function(d){ return(sliderStart + maxWidth * 0.15 + d.value * maxWidth)})
     workerLabs.text(function(d) { return(Math.round(d.value * 200))})
     salaryLabs.attr("x", function(d){ return(sliderStart + maxWidth * 0.15 + d.value * maxWidth)})
     salaryLabs.text(function(d) { return("£" + Math.round(d.value * 500) + "k")})
}


var barScale = d3.drag()
               .on("drag", barDrag)
               .on("start", barDrag)
               .on("end", updatePlot);

maxWidth = (sliderEnd -  sliderStart) * 0.8;

// Scales for the workers plot
var xW = d3.scaleLinear()
           .domain([0, 200])
           .range([sliderStart + (maxWidth) / 20, sliderEnd - (maxWidth) / 20]);
var yW = d3.scaleBand()
           .domain([0, 1, 2, 3])
           .range([y(0.65), y(0.45)])

// Create draggable bars for inputting
var workerheight = h / 25.6;

var workers2 = [{position: "A", value: 11 / maxWorkers},
                {position: "B", value: 17 / maxWorkers},
                {position: "C", value: 59 / maxWorkers},
                {position: "D", value: 115 / maxWorkers}];


var workerBars =  svg_bar.selectAll(".worker")
                         .data(workers2)
                         .enter().append("rect")
                         .attr("class", "worker")
                         .attr("y", function(d, i) {return(yW(i))})
                         .attr("x", sliderStart + maxWidth * 0.1 )
                         .attr("width", function(d, i) {return(d.value * maxWidth)})
                         .attr("height", workerheight)
                         .attr("fill", malecol)
                         .call(barScale);

var workerAxes = svg_bar.selectAll("workeraxes")
                        .data(workers2)
                        .enter().append("text")
                        .attr("class", "workeraxes")
                        .text(function(d){ return d.position})
                        .attr("x", xW(- 15))
                        .attr("y", function(d, i){ return yW(i) + y(0.99)})
                        .attr("fill", malecol)
                        .attr("text-anchor", "right")
                        .attr("font-family", "sans-serif")
                        .attr("font-size", "12px")
                        .attr("pointer-events", "none");

var workerLabs = svg_bar.selectAll("workerLabs")
                        .data(workers2)
                        .enter()
                        .append("text")
                        .attr("class", "workerlabs")
                        .attr("x", function(d){ return(sliderStart + maxWidth * 0.15 + d.value * maxWidth) })
                        .attr("y", function(d, i) {return yW(i) + workerheight * 0.75})
                        .text(function(d) { return Math.round(d.value * 200)})
                        .attr("fill", malecol)
                        .attr("text-anchor", "left")
                        .attr("font-family", "sans-serif")
                        .attr("font-size", "12px")
                        .attr("pointer-events", "none");
var workersText = svg_bar.append("text")
                         .text("No. of workers")
                         .attr("x", xW(100))
                         .attr("y", yW(0) - y(0.99))
                         .attr("class", "genText")
                         .attr("text-anchor", "middle")
                         .attr("font-size", "12px")

// Add draggable bars for changing salary levels
var salaries2 = [{position: "A", value: 500000 / maxSalary},
                 {position: "B", value: 125000 / maxSalary},
                 {position: "C", value: 60000 / maxSalary},
                 {position: "D", value: 20000 / maxSalary}];

var salaryBar = svg_bar.selectAll(".salary.bars")
                       .data(salaries2)
                       .enter()
                       .append("rect")
                       .attr("class", "salary bars")
                       .attr("y", function(d, i) {return(yW(i) + y(0.66))})
                       .attr("x", sliderStart + maxWidth * 0.1)
                       .attr("width", function(d, i) {return(d.value * maxWidth)})
                       .attr("height", workerheight)
                       .attr("fill", femalecol)
                       .call(barScale);

var salaryLabs = svg_bar.selectAll(salaryLabs)
                        .data(salaries2)
                        .enter()
                        .append("text")
                        .attr("class", "salarylabs")
                        .attr("x", function(d){ return(sliderStart + maxWidth * 0.15 + d.value * maxWidth) })
                        .attr("y", function(d, i) {return yW(i) + y(0.66) + workerheight * 0.75})
                        .text(function(d) { return "£" + Math.round(d.value * 500) + "k"})
                        .attr("fill", femalecol)
                        .attr("text-anchor", "left")
                        .attr("font-family", "sans-serif")
                        .attr("font-size", "12px")
                        .attr("pointer-events", "none");

var salariesText = svg_bar.append("text")
                       .text("Salaries")
                       .attr("x", xW(100))
                       .attr("y", yW(0) - y(0.99) + y(0.66))
                       .attr("class", "genText")
                       .attr("text-anchor", "middle")
                       .attr("font-size", "12px");

var salaryAxes = svg_bar.selectAll("salaryaxes")
                        .data(workers2)
                        .enter().append("text")
                        .attr("class", "salaryaxes")
                        .text(function(d){ return d.position})
                        .attr("x", xW(- 15))
                        .attr("y", function(d, i){ return yW(i) + y(0.66) + y(0.99)})
                        .attr("fill", femalecol)
                        .attr("text-anchor", "right")
                        .attr("font-family", "sans-serif")
                        .attr("font-size", "12px")
                        .attr("pointer-events", "none");

// The slider for selecting gender proportions
var sliderLine = svg_bar.append("line")
                        .attr("x1", sliderStart)
                        .attr("x2", sliderEnd)
                        .attr("y1", h * 0.18)
                        .attr("y2", h * 0.18)
                        .attr("stroke", femalecol)
                        .attr("class", "sliderLine")
                        .call(drag);

var sliderCircle = svg_bar.append("circle")
                          .attr("cx", xW(100))
                          .attr("cy", h * 0.18)
                          .attr("r", 7)
                          .attr("fill", malecol)
                          .attr("stroke", "#000000")
                          .attr("class", "sliderCircle")
                          .call(drag);

var sliderText = svg_bar.append("text")
                        .text("Female applicants : 50%")
                        .attr("x", xW(100))
                        .attr("y", h * 0.18 - y(0.99))
                        .attr("class", "genText")
                        .attr("text-anchor", "middle")
                        .attr("font-size", "12px")
                        .call(drag);




// Add attribution
svg_bar.append("text")
       .attr("x", margin[1])
       .attr("y", h)
       .attr("text-anchor", "right")
       .attr("class", "genText")
       .attr("fill", "#ACACAC")
       .attr("font-family", "Open Sans")
       .text("Source: www.nathancunn.com (@nathcun)");

// Add title
svg_bar.append("text")
       .attr("x", xScale(-145))
       .attr("y", y(1) + 10)
       .attr("text-anchor", "right")
       .attr("fill", "#888888")
        .attr("font-family", "Roboto")
        .attr("font-size", "22px")
        .attr("font-weight", "bold")
        .text("How likely is a pay gap to occur?");

svg_bar.append("g")
       .attr("class", "x axis")
       .call(xAxis)
       .attr("transform", "translate(0," + (h - margin[2]) + ")");
svg_bar.append("g")
       .attr("class", "y axis")
       .call(yAxis)
       .attr("transform", "translate(" + margin[3] + ", 0)")

// text label for the x axis
svg_bar.append("text")
       .text("→ % pay gap (favouring men)")
       .attr("text-anchor", "start")
       .attr("x", xScale(0))
       .attr("y", h - margin[2] / 2.5)
       .attr("class", "genText")
       .attr("fill", malecol);
svg_bar.append("text")
      .text("% pay gap (favouring women)←")
      .attr("text-anchor", "end")
      .attr("x", xScale(0))
      .attr("y", h - margin[2] / 2.5)
      .attr("class", "genText")
      .attr("fill", femalecol);
// text label for y axis
svg_bar.append("text")
       .attr("transform", "rotate(-90)")
       .attr("y", margin[3] / 10)
       .attr("x",0 - (h - margin[0] - margin[2]) / 2)
       .attr("dy", "1em")
       .attr("class", "genText")
       .style("text-anchor", "middle")
       .text("Frequency (%)");
    </script>
