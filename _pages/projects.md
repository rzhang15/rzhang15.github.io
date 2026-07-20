---
layout: page
title: Research
permalink: /research/
description:
nav: true
nav_order: 2
---

<style>
  /* Site accent / link color (overrides the theme's default magenta). */
  :root {
    --global-theme-color: #0076df;
    --global-hover-color: #0076df;
  }
  html[data-theme="dark"] {
    --global-theme-color: #58a6ff;
    --global-hover-color: #58a6ff;
  }
  /* Paper entries */
  .paper-card {
    margin-bottom: 1.75rem;
  }
  .paper-card .paper-authors,
  .paper-card .paper-venue {
    font-size: 0.9rem;
  }
  .paper-card details {
    margin-top: 0.4rem;
  }
  .paper-card summary {
    display: inline-block;
    cursor: pointer;
    list-style: none;
    font-size: 0.9rem;
    color: var(--global-theme-color);
  }
  .paper-card summary::-webkit-details-marker {
    display: none;
  }
  .paper-card summary::after {
    content: " ▸";
  }
  .paper-card details[open] summary::after {
    content: " ▾";
  }
  .paper-card summary:hover {
    text-decoration: underline;
  }
  .paper-card .abstract-body {
    margin-top: 0.5rem;
    text-align: justify;
  }
  .paper-card .paper-extra {
    margin-top: 0.5rem;
    font-size: 0.85rem;
    color: var(--global-text-color-light);
  }
</style>

<script>
  (function () {
    var links = document.querySelectorAll("a.nav-link");
    var cvLink = null;
    for (var i = 0; i < links.length; i++) {
      var href = links[i].getAttribute("href") || "";
      if (/\/cv\/?($|[?#])/i.test(href)) {
        cvLink = links[i];
        break;
      }
    }
    if (!cvLink) return;
    cvLink.addEventListener("click", function (e) {
      e.preventDefault();
      window.open("/assets/pdf/Ruby (Ruishan) Zhang Curriculum Vitae.pdf", "_blank", "noopener");
    });
  })();
</script>

## Job Market Paper

<div class="paper-card">
<b>The Returns to Science of Centrally Provisioned GPUs and Optimal Allocation</b><br>
<span class="paper-authors">(with <a href="https://conniexu75.github.io/">Connie Xu</a>)</span>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>Artificial intelligence and deep learning methods require expensive capital investments in the form of Graphical Processing Units (GPUs). Given the importance of GPU clusters to computational research, where should infrastructure funding be allocated? We construct a novel panel of university GPU capacity and research output for R1 U.S. universities, combining historical snapshots of research computing websites with bibliometric data from OpenAlex. We use large, discrete computing capacity jumps in an event-study design and find modest effects of cluster upgrades on AI-related publications. However, there is significant heterogeneity: low-tier universities exhibit a larger marginal response to capacity upgrades than high-tier universities. We develop a structural model of the university as a multi-product organization to estimate the production function for GPU-enabled research, derive a capital allocation rule across fields, and use the estimated elasticities to characterize the NSF's revealed preference over efficiency versus equity. Our findings suggest that diminishing returns to computing capital favor a more redistributive allocation of federal cyberinfrastructure grants.</p>
</div>
</details>
</div>

## Working Papers

<div class="paper-card">
<b>Secrecy, Spectrum, and Certification: Evidence from Wireless Electronic Devices</b><br>
<span class="paper-authors">(with <a href="https://scholar.google.com/citations?user=KjdWS1kAAAAJ&hl=en">Roberto Fontana</a>, <a href="https://www.hbs.edu/faculty/Pages/profile.aspx?facId=718917">Shane Greenstein</a>, and <a href="https://scholar.google.com/citations?user=PWNDHjgAAAAJ&hl=en">Do Yoon Kim</a>)</span>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>This paper examines the strategic decisions of firms to withhold information in innovation-intensive markets, highlighting that secrecy contains distinct temporal dimensions. Using all FCC equipment filings from 2001 to 2021, we analyze firms' choices between long-term confidentiality (LTC), which permanently conceals technical information such as block diagrams, and short-term confidentiality (STC), which temporarily delays the public release of marketing information to ensure against launch and coordination risks in the commercialization process. LTC use reflects appropriability concerns and institutional complexities—technically complex products and competitive markets are 12 to 35% more likely to adopt it. By contrast, STC is driven by the commercialization timing of branded products by large firms. Large, domestic, patent-owning firms with regulatorily complex products are more likely to use STC. Technical aspects of the product do not predict STC usage. An exposure-based event study further shows that firms with a high ex-ante propensity to use STC bring products to market faster after the policy becomes available, with no corresponding changes in product complexity or volume.</p>
</div>
</details>
</div>

<div class="paper-card">
<b>Scientific Input Costs in University Life Sciences Research</b><br>
<span class="paper-authors">(with <a href="https://conniexu75.github.io/">Connie Xu</a>)</span>
<!-- <details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>Public funders delegate money and broad discretion to principal investigators (PIs), yet whether that discretion protects research output when input prices rise is unknown. We ask how PIs adjust, and how much research is lost. Using novel purchase-level procurement records, we exploit the 2014 merger of Thermo Fisher Scientific and Life Technologies as a shock to input prices. A matched difference-in-differences design estimates that prices in affected markets rose approximately 20 percent while quantities moved minimally, indicating highly inelastic demand. Tracing this cost shock through a panel of 6,382 U.S. life sciences PIs, we find the average PI, facing a 3.2 percent rise in input costs, publishes about 1.2 percent fewer papers, an elasticity of about -0.38. The decline concentrates among early-career PIs, who command fewer resources to draw on. The volume of publicly funded science thus depends on prices in input markets and on the PIs who manage the grants.</p>
</div>
</details> -->
</div>

## Publications

<div class="paper-card">
<b><a href="https://doi.org/10.1016/j.telpol.2026.103209">Wireless communications equipment markets: evolution, classification, and measurement</a></b><br>
<span class="paper-authors">(with <a href="https://www.linkedin.com/in/noah-greenstein-aa0872133/">Noah Greenstein</a>, <a href="https://scholar.google.com/citations?user=KjdWS1kAAAAJ&hl=en">Roberto Fontana</a>, <a href="https://www.hbs.edu/faculty/Pages/profile.aspx?facId=718917">Shane Greenstein</a>, <a href="https://haiyangzhang.org/">Haiyang Zhang</a>, <a href="https://omarolivarez.com/">Omar Olivarez</a>, and <a href="https://scholar.google.com/citations?user=PWNDHjgAAAAJ&hl=en">Do Yoon Kim</a>)</span><br>
<span class="paper-venue"><i>Telecommunications Policy</i>, 2026.</span>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>A central concern of many policy debates has been to foster more innovative wireless markets. How can policymakers assess whether this objective has been achieved? One measure of successful innovation is an increase in the breadth of markets addressed by new products. Existing product taxonomies, such as the North American Industry Classification System (NAICS), require new products to fit into legacy categories. Thus, they may fail to fully measure the development of new products from emerging wireless markets. This study proposes an experimental product code based on the compliance and certification applications for over 200,000 wireless devices in the Federal Communications Commission's (FCC) Equipment Authorization System (EAS) database from 1982 to 2021. The taxonomy was developed using a novel methodology, in which key phrases from application product descriptions were matched to product categories. The product code is inspired by, but diverges from, the NAICS codes. It comprises three levels of nested product aggregation: 26 Classes, 83 Families, and 298 Types, offering unique avenues to analyze the cross-market scope of wireless technology over decades. The study shows that the breadth of markets for wireless products has grown over time, particularly in areas supported by unlicensed spectrum and corresponding standards, such as Wi-Fi and Bluetooth.</p>
</div>
</details>
</div>

<div class="paper-card">
<b><a href="https://doi.org/10.1038/s41586-022-04996-4">Social capital I: measurement and associations with economic mobility</a></b><br>
<span class="paper-authors">(with <a href="https://www.economics.harvard.edu/people/raj-chetty">Raj Chetty</a>, <a href="https://web.stanford.edu/~jacksonm/">Matthew O. Jackson</a>, <a href="https://pages.stern.nyu.edu/~tkuchler/">Theresa Kuchler</a>, <a href="https://pages.stern.nyu.edu/~jstroebe/">Johannes Stroebel</a>, et al.)</span><br>
<span class="paper-venue"><i>Nature</i>, 2022.</span>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>Social capital—the strength of an individual's social network and community—has been identified as a potential determinant of outcomes ranging from education to health. However, efforts to understand what types of social capital matter for these outcomes have been hindered by a lack of social network data. Here, in the first of a pair of papers, we use data on 21 billion friendships from Facebook to study social capital. We measure and analyse three types of social capital by ZIP (postal) code in the United States: (1) connectedness between different types of people, such as those with low versus high socioeconomic status (SES); (2) social cohesion, such as the extent of cliques in friendship networks; and (3) civic engagement, such as rates of volunteering. These measures vary substantially across areas, but are not highly correlated with each other. We demonstrate the importance of distinguishing these forms of social capital by analysing their associations with economic mobility across areas. The share of high-SES friends among individuals with low SES—which we term economic connectedness—is among the strongest predicters of upward income mobility identified to date. Other social capital measures are not strongly associated with economic mobility. If children with low-SES parents were to grow up in counties with economic connectedness comparable to that of the average child with high-SES parents, their incomes in adulthood would increase by 20% on average. Differences in economic connectedness can explain well-known relationships between upward income mobility and racial segregation, poverty rates, and inequality. To support further research and policy interventions, we publicly release privacy-protected statistics on social capital by ZIP code at https://www.socialcapital.org.</p>
</div>
</details>
<div class="paper-extra">Media coverage: <a href="https://www.nytimes.com/interactive/2022/08/01/upshot/rich-poor-friendships.html">New York Times</a></div>
</div>

<div class="paper-card">
<b><a href="https://doi.org/10.1038/s41586-022-04997-3">Social capital II: determinants of economic connectedness</a></b><br>
<span class="paper-authors">(with <a href="https://www.economics.harvard.edu/people/raj-chetty">Raj Chetty</a>, <a href="https://web.stanford.edu/~jacksonm/">Matthew O. Jackson</a>, <a href="https://pages.stern.nyu.edu/~tkuchler/">Theresa Kuchler</a>, <a href="https://pages.stern.nyu.edu/~jstroebe/">Johannes Stroebel</a>, et al.)</span><br>
<span class="paper-venue"><i>Nature</i>, 2022.</span>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>Low levels of social interaction across class lines have generated widespread concern and are associated with worse outcomes, such as lower rates of upward income mobility. Here we analyse the determinants of cross-class interaction using data from Facebook, building on the analysis in our companion paper. We show that about half of the social disconnection across socioeconomic lines—measured as the difference in the share of high-socioeconomic status (SES) friends between people with low and high SES—is explained by differences in exposure to people with high SES in groups such as schools and religious organizations. The other half is explained by friending bias—the tendency for people with low SES to befriend people with high SES at lower rates even conditional on exposure. Friending bias is shaped by the structure of the groups in which people interact. For example, friending bias is higher in larger and more diverse groups and lower in religious organizations than in schools and workplaces. Distinguishing exposure from friending bias is helpful for identifying interventions to increase cross-SES friendships (economic connectedness). Using fluctuations in the share of students with high SES across high school cohorts, we show that increases in high-SES exposure lead low-SES people to form more friendships with high-SES people in schools that exhibit low levels of friending bias. Thus, socioeconomic integration can increase economic connectedness in communities in which friending bias is low. By contrast, when friending bias is high, increasing cross-SES interactions among existing members may be necessary to increase economic connectedness. To support such efforts, we release privacy-protected statistics on economic connectedness, exposure and friending bias for each ZIP (postal) code, high school and college in the United States at https://www.socialcapital.org.</p>
</div>
</details>
<div class="paper-extra">Media coverage: <a href="https://www.nytimes.com/2022/08/01/briefing/economic-ladder-rich-poor-americans.html">New York Times</a></div>
</div>

## Policy Writing

<div class="paper-card">
<b><a href="https://nap.nationalacademies.org/resource/27838/Zhang_Commissioned_Paper.pdf">Building Up Research Capacity at Minority Institutions</a></b>
<details>
<summary>Abstract</summary>
<div class="abstract-body">
<p>This paper aims to characterize the current research capacity of Minority Institutions (MIs) and explore potential investment avenues, using survey data from the National Science Foundation (NSF). The paper compares MIs to institutions with very high research activity (R1) and high research activity (R2) as classified by the Carnegie Classification of Institutions of Higher Education (CCIHE). The analysis examines where MIs currently stand in the Carnegie Classification, and how they compare to R1s/R2s in terms of research and development (R&D) expenditure and facility space broken down by field. However, due to left truncation in the data, while R1s/R2s are well represented, the selection focuses on the highest-spending MIs. Despite the missing data problems, only by first understanding the current state of research using the best available public data can forward-looking policy suggestions then be made. To that end, it is important to keep in mind and understand what the institution objectives are, and under what framework institutions operate. This paper first describes the institution types, to inform readers of the different objectives that institutions may have.</p>
</div>
</details>
<div class="paper-extra">NAS Commissioned Paper: <a href="https://www.nationalacademies.org/projects/PGA-POLICY-22-17">A Plan to Promote Defense Research at Minority-Serving Institutions</a></div>
</div>
