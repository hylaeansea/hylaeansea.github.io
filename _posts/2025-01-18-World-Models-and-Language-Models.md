---
layout: post
title:  "World Models and Language Models, a Philosophy"
date:   2025-01-18 08:17:00 +0000
categories: blog
---

<style>
.prompt-box {
    border: 2px solidrgb(54, 56, 54); 
    padding: 10px; 
    border-radius: 5px; 
    background-color:rgb(215, 191, 255); 
    box-shadow: 2px 2px 5px rgba(0, 0, 1, 0.1);
}
.chatgpt-4o-box {
    border: 2px solidrgb(54, 56, 54); 
    padding: 10px; 
    border-radius: 5px; 
    background-color:rgb(202, 235, 194); 
    box-shadow: 2px 2px 5px rgba(0, 0, 1, 0.1);
}
.llama-box {
    border: 2px solidrgb(54, 56, 54); 
    padding: 10px; 
    border-radius: 5px; 
    background-color:rgb(209, 209, 209); 
    box-shadow: 2px 2px 5px rgba(0, 0, 1, 0.1);
}
</style>



# Abstract


![Computable Policy]({{ site.baseurl }}/assets/images/DALL·E_2025-01-18_11.27.13-A_futuristic_and_realistic_scene_depicting_the_concept_of_computable_policy.webp) 
*Image generated with DALL·E; prompt: make a futuristic but realistic image that exemplifies "computable policy" as you have just described*


# Introduction

Through the course of this project, I attempted to answer the question: 

***Can we make policy computable?***

I conjecture that many of the tasks that Large Language Models are relatively good at, tend to also be relatively easy to verify the correctness of the output. Testing whether code compiles, having a bilingual human verify a translation, determining if re-written prose sounds better, or a generated poem conforms to rhyme and meter, are all tasks that can be done by humans with relative ease or verified computationally with relative ease.

The other major factor in the quality of an LLM response, is of course the prevalence of a large volume of high quality training data. The examples above also satisfy this criteria; many examples of code that compiles, many examples of well written prose, and many examples of good poetry that conforms to the standards of the craft.

However, as we are rapidly progressing to near ubiquitous proliferation of LLMs in our economy, technology, society, and even government, the outputs of LLMs for these tasks is not immediately computable. Consider the response to the following prompt:

<div class="prompt-box">
<b>Prompt</b>: What are key elements of a public policy to maximize the uptake and adoption of AI technology by the maximum number of people? Be Specific.
</div>

Some example responses include:

<div class="chatgpt-4o-box">
    <b>ChatGPT 4o</b>: Its response focuses on Education, Accessibility, Infrastructure, Trust, Public Awareness, and other suggestions. These categories have a couple of simple bullet points, however this response remains high level.

<details>
  <summary>
    Click here for full text of response
  </summary>
<hr>
Key Elements of a Public Policy to Maximize AI Adoption
<br>
<h3>1. Education and Skills Development</h3>
<ul>
    <li><strong>AI Literacy Programs:</strong> Introduce AI literacy in school curricula and adult education programs to demystify the technology.</li>
    <li><strong>Reskilling Initiatives:</strong> Provide training and certifications in AI-related skills for workers displaced by automation.</li>
    <li><strong>Community Workshops:</strong> Offer free or low-cost workshops and online courses tailored to different demographics, especially underserved communities.</li>
</ul>

<h3>2. Accessibility and Affordability</h3>
<ul>
    <li><strong>Subsidies for AI Tools:</strong> Provide financial assistance or tax incentives for small businesses and individuals to purchase AI software and hardware.</li>
    <li><strong>Open-Source Initiatives:</strong> Promote the development and availability of open-source AI tools and platforms.</li>
    <li><strong>Digital Inclusion Programs:</strong> Expand access to the internet and devices in rural and low-income areas.</li>
</ul>

<h3>3. Infrastructure Development</h3>
<ul>
    <li><strong>High-Speed Internet:</strong> Invest in nationwide broadband infrastructure to ensure equitable access.</li>
    <li><strong>Cloud Computing Resources:</strong> Provide access to shared computing resources, such as public AI supercomputing hubs.</li>
    <li><strong>Data Sharing Frameworks:</strong> Create secure and ethical data-sharing platforms to support AI innovation.</li>
</ul>

<h3>4. Trust and Ethics</h3>
<ul>
    <li><strong>Regulation of Bias and Fairness:</strong> Enforce clear guidelines to reduce bias in AI algorithms and ensure fair outcomes.</li>
    <li><strong>Transparent AI Policies:</strong> Mandate that organizations disclose how AI systems make decisions.</li>
    <li><strong>Consumer Protections:</strong> Develop robust policies for data privacy, security, and accountability.</li>
</ul>

<h3>5. Financial Incentives</h3>
<ul>
    <li><strong>Tax Credits:</strong> Offer tax benefits to businesses that adopt AI technologies for productivity or innovation.</li>
    <li><strong>Grants for Startups:</strong> Provide funding to AI startups and small businesses to encourage experimentation and deployment.</li>
    <li><strong>Public-Private Partnerships:</strong> Foster collaborations between government, academia, and industry to lower the costs of AI adoption.</li>
</ul>

<h3>6. Public Awareness Campaigns</h3>
<ul>
    <li><strong>Showcase Success Stories:</strong> Highlight how AI is being used to solve real-world problems in diverse fields such as healthcare, agriculture, and education.</li>
    <li><strong>Address Fears:</strong> Run campaigns that address concerns about job displacement and AI risks, focusing on its potential benefits.</li>
</ul>

<h3>7. Sector-Specific Support</h3>
<ul>
    <li><strong>Tailored Adoption Programs:</strong> Develop sector-specific AI adoption guidelines and tools (e.g., for healthcare, education, manufacturing).</li>
    <li><strong>Incubators and Sandboxes:</strong> Establish environments where businesses can test AI solutions under regulatory guidance.</li>
</ul>

<h3>8. Inclusive Design and Participation</h3>
<ul>
    <li><strong>Localized Solutions:</strong> Support AI development tailored to local languages, cultural norms, and regional needs.</li>
    <li><strong>Community Involvement:</strong> Involve diverse stakeholders, including marginalized communities, in the design and implementation of AI policies.</li>
</ul>

<h3>9. Incentivizing Research and Development</h3>
<ul>
    <li><strong>Academic Funding:</strong> Increase funding for AI research in public universities and institutions.</li>
    <li><strong>Cross-Border Collaboration:</strong> Partner with international entities to share knowledge and resources.</li>
</ul>

<h3>10. Monitoring and Evaluation</h3>
<ul>
    <li><strong>Impact Assessment Frameworks:</strong> Continuously evaluate the societal and economic impact of AI adoption.</li>
    <li><strong>Feedback Mechanisms:</strong> Set up channels for public feedback to iteratively improve AI policies.</li>
</ul>

<h3>Implementation Strategy</h3>
<ul>
    <li><strong>Pilot Programs:</strong> Roll out pilot projects in targeted communities to test policies and adjust based on outcomes.</li>
    <li><strong>Scalable Models:</strong> Focus on scalable models for AI deployment to maximize reach.</li>
</ul>

<h3>Legal and Policy Support</h3>
<ul>
    <li><strong>Legal Frameworks:</strong> Simplify compliance requirements for AI technology adoption while maintaining ethical standards.</li>
    <li><strong>AI Ombudsman:</strong> Create an independent body to address grievances and ensure fair AI implementation.</li>
</ul>


</details>

</div>



<div class="llama-box">

<b>llama3.1:8b</b> provided fewer focus elements than <b>o4</b>, however they were similar: Education, Infrastructure, Regulation, and Economic Incentives. Similarly to <b>4o</b>, <b>llama3.1:8b</b> remains at a high level without much detail.

<details>
  <summary>
    Click here for full text of response
  </summary>
    <hr>
    To maximize the uptake and adoption of AI technology by the maximum number of people, a public policy should include the following key elements:
    <br>
    <h3><strong>I. Infrastructure and Accessibility</strong></h3>
    <ol>
        <li><strong>Universal Broadband</strong>: Ensure that all households have access to high-speed internet (at least 100 Mbps) to facilitate AI-powered applications.</li>
        <li><strong>Digital Literacy Training</strong>: Provide training programs for individuals to develop basic digital skills, including understanding of AI concepts and how to use AI-enabled devices.</li>
        <li><strong>Accessibility Standards</strong>: Implement accessibility standards for AI systems, ensuring that they can be used by people with disabilities.</li>
    </ol>

    <h3><strong>II. Education and Awareness</strong></h3>
    <ol>
        <li><strong>AI Education in Schools</strong>: Integrate AI education into school curricula, starting from primary level, to foster a generation of AI-literate individuals.</li>
        <li><strong>Public Awareness Campaigns</strong>: Launch public awareness campaigns to educate citizens about the benefits, risks, and applications of AI technology.</li>
        <li><strong>Research Grants</strong>: Provide research grants for academia and industry to develop AI-related educational materials and programs.</li>
    </ol>

    <h3><strong>III. Regulations and Governance</strong></h3>
    <ol>
        <li><strong>Clear AI Regulations</strong>: Establish clear regulations and guidelines for AI development, deployment, and use in various sectors (e.g., healthcare, finance).</li>
        <li><strong>Data Protection and Privacy</strong>: Strengthen data protection laws and regulations to safeguard citizens' personal data used by AI systems.</li>
        <li><strong>Transparency and Accountability</strong>: Mandate transparency in AI decision-making processes and hold developers accountable for AI-related errors or harm.</li>
    </ol>

    <h3><strong>IV. Economic and Social Incentives</strong></h3>
    <ol>
        <li><strong>Tax Incentives</strong>: Offer tax incentives to businesses that invest in AI research, development, and deployment.</li>
        <li><strong>Job Training Programs</strong>: Develop job training programs to upskill workers in areas where AI is transforming industries (e.g., manufacturing, customer service).</li>
        <li><strong>Social Benefits</strong>: Provide social benefits, such as subsidies or vouchers, for low-income individuals who want to access AI-enabled services.</li>
    </ol>

    <h3><strong>V. Collaboration and Partnerships</strong></h3>
    <ol>
        <li><strong>Public-Private Partnerships</strong>: Foster partnerships between government agencies, industry leaders, and academia to drive AI innovation and adoption.</li>
        <li><strong>AI Ecosystem Development</strong>: Encourage the development of AI ecosystems in various regions, promoting collaboration among startups, researchers, and businesses.</li>
        <li><strong>Global Cooperation</strong>: Engage in international collaborations to establish global standards for AI development, deployment, and use.</li>
    </ol>

    <h3><strong>VI. Monitoring and Evaluation</strong></h3>
    <ol>
        <li><strong>Impact Assessment</strong>: Conduct regular impact assessments to evaluate the effectiveness of public policies on AI adoption and usage.</li>
        <li><strong>Data Collection</strong>: Establish a data collection framework to monitor AI-related trends, challenges, and best practices.</li>
        <li><strong>Continuous Review and Update</strong>: Regularly review and update policies as new evidence emerges or as AI technology evolves.</li>
    </ol>

    <p>By incorporating these key elements, a public policy can effectively support the widespread adoption of AI technology and maximize its benefits for society as a whole.</p>
</details>
</div>



These responses are coherent, have good diverse suggestions, and seem like they would be good public policy recommendations to increase the general public's understanding and use of emerging AI. However, they lack specific policy details like funding levels, distribution of tech and benefits amongst society, the ability to deal with specific alignment issues, and the relationship between AI companies, the public, and regulating bodies. This is not a critique of these initial responses, and the next logical prompt would be to focus on a specific area of the policy and refine the details.

If we look at prompts to focus on AI education but for two different cities, we see largely similar responses.

<div class="prompt-box">
provide a specific policy for the increasing of education on AI for <b>Denver</b> Public Schools, focus on program cost, student admittance, whether it should focus on low and middle income schools, use of other resources in the community and provide hurdles to this implementation, please write the response in html with the highest level of header being h2
</div>

<div class="chatgpt-4o-box">
<b>ChatGPT-4o</b> - Policy for Expanding AI Education in Denver Public Schools
<details>
<summary>
Cost, Admission, Community Resources, Hurdles
</summary>
    <h3>Program Cost</h3>
    <p>The estimated cost for the program is $2.5 million annually. This includes curriculum development, teacher training, purchasing technology (computers, AI software), and funding extracurricular activities such as AI clubs or hackathons. Additional funding will be allocated for partnerships with local tech companies and universities.</p>

    <h3>Student Admittance</h3>
    <p>Admission to the program will be open to all students in Denver Public Schools. However, priority will be given to students from low- and middle-income backgrounds to ensure equitable access to AI education. Outreach efforts will focus on underrepresented groups in STEM fields, including girls and minorities.</p>

    <h3>Focus on Low and Middle-Income Schools</h3>
    <p>The program will initially target low and middle-income schools where access to technology and advanced STEM education is limited. By addressing educational disparities, the program aims to bridge the digital divide and prepare students for future opportunities in AI-related fields.</p>

    <h3>Utilizing Community Resources</h3>
    <ul>
        <li><strong>Local Tech Companies:</strong> Collaborate with tech firms in Denver to provide mentorship, internships, and funding for resources.</li>
        <li><strong>Universities:</strong> Partner with the University of Colorado and other institutions to develop a robust AI curriculum and offer dual-enrollment courses.</li>
        <li><strong>Community Centers:</strong> Use existing community centers to host AI workshops and provide after-school programs.</li>
        <li><strong>Nonprofits:</strong> Work with nonprofit organizations focused on STEM education to secure grants and additional resources.</li>
    </ul>

    <h3>Hurdles to Implementation</h3>
    <ul>
        <li><strong>Funding:</strong> Securing sustainable funding may be challenging due to budget constraints and competing priorities within the school district.</li>
        <li><strong>Teacher Training:</strong> There may be a shortage of educators with the expertise to teach AI effectively, necessitating significant investment in professional development.</li>
        <li><strong>Infrastructure:</strong> Many schools, especially in low-income areas, may lack the necessary technology infrastructure to support AI education.</li>
        <li><strong>Community Buy-In:</strong> Gaining support from parents, teachers, and local stakeholders may require extensive outreach and demonstration of the program's value.</li>
        <li><strong>Equity Challenges:</strong> Ensuring equitable access and avoiding unintentional exclusion of marginalized groups will require careful planning and oversight.</li>
    </ul>
</details>
</div>

<div class="prompt-box">
provide a specific policy for the increasing of education on AI for <b>Boulder</b> Public Schools, focus on program cost, student admittance, whether it should focus on low and middle income schools, use of other resources in the community and provide hurdles to this implementation, please write the response in html with the highest level of header being h2
</div>

<div class="chatgpt-4o-box">
<b>ChatGPT-4o</b> - Policy for Expanding AI Education in Boulder Public Schools
<details>
<summary>
Cost, Admission, Equity, Community Resources, Hurdles
</summary>

    <h2>AI Education Policy for Boulder Public Schools</h2>

    <h3>Program Cost</h3>
    <p>
        The program is estimated to cost $500,000 annually, with funding allocated to teacher training, AI curriculum development, and equipment such as computers and software licenses. Grants from technology companies and state educational funds should be pursued to reduce the burden on the school district.
    </p>

    <h3>Student Admittance</h3>
    <p>
        The program should initially target middle and high school students with demonstrated interest in technology and science. Admission will be determined by teacher recommendations, application essays, and interest surveys to ensure students' commitment.
    </p>

    <h3>Focus on Low and Middle-Income Schools</h3>
    <p>
        The policy will prioritize low and middle-income schools to bridge the digital divide. Schools in these areas will receive additional resources, including outreach initiatives to inform students and parents about the benefits of AI education.
    </p>

    <h3>Use of Other Resources in the Community</h3>
    <p>
        Partnerships with local universities, tech companies, and libraries will provide additional support. These resources may include guest lectures, internships, AI-focused workshops, and access to advanced computing facilities.
    </p>

    <h3>Hurdles to Implementation</h3>
    <ul>
        <li><strong>Funding:</strong> Securing consistent funding from public and private sources could be challenging.</li>
        <li><strong>Teacher Training:</strong> Current staff may lack the expertise to teach AI concepts, requiring extensive professional development.</li>
        <li><strong>Curriculum Development:</strong> Crafting a relevant and engaging curriculum will take time and specialized knowledge.</li>
        <li><strong>Equity:</strong> Ensuring all students have access to necessary hardware and internet connectivity at home may be difficult.</li>
        <li><strong>Community Buy-In:</strong> Gaining support from parents, teachers, and administrators may require significant effort to highlight the program's benefits.</li>
    </ul>

    <p>
        Implementing AI education in Boulder Public Schools will require careful planning and collaboration with community partners. By addressing funding and training challenges while focusing on equity, the district can create a robust program that benefits students and prepares them for future careers.
    </p>

</details>

</div>
<br>

# Motivation
We can see from these responses to nearly identical prompts that there are possibly some relevant differences, like cost for the different sized populations, a slight difference in low and middle income emphasis, and some more detail (or at least different formatting) for the engagement of community resources. However, reflecting on my original conjecture:

* *How do we know how well these policies will work?*
* *What accounts for the differences between the policies for different municipalities?*
* *Is there a better way to bake this knowledge into our LLMs, rather than whole internet base training, followed by fine tuning and alignment?*
* In short: ***Can we make policy computable?***


## Why would computable policy be useful?

## Existing work on computable policy and world models

# Methods of Investigation

# Results

# Discussion

## What does this mean for safety

Talk about agentic and a diversity of specifically fine tuned models

# Future Work

## Ocean Biodiversity and Conservation

## Space Policy


