<svelte:head>
	<title>Home</title>
	<meta name="description" content="home page" />
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
	<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap" rel="stylesheet">
</svelte:head>

<h1>
	PhishBusters
</h1>
<hr>
<br>

<div class="background-div">
	<div class="row">
		<div class="three-column">
			<p class=p-header>Project Description</p>
			<p style="padding:10px;">PhishBusters is an easy to understand website aimed to inform users about different types of scams. It was built using CSS, HTML, and JavaScript through the Svelte framework. This website is aimed at users that are looking for information about how to detect scams, people who suspect they’re being scammed, and internet users unfamiliar with how to safely navigate the web. We have information on two types of phishing attacks called .zip domains and web skimming.</p>
		</div>
		<div class="three-column">
			<p class=p-header>About the Team</p>
			<p style="padding:10px;">We are the Phishbusters, your trusted cybersecurity force. We’re here to keep you safe on the web by spreading awareness about phishing attempts and other cybersecurity attacks. We are a team of four externs developing a project for the ALRISE 2023 Summer Externship Program. We have two researchers, Giovani Castillo and Paris Saucedo, and two web developers, Mateo Estrada and Casandra Marquez.</p>
		</div>
		<div class="three-column">
			<p class=p-header>Why it Matters</p>
			<p style="padding:10px;">All it takes is better judgment and vigilance when browsing the internet to stay safe. Our goal is to spread information to avoid scammers from having an upper hand and taking advantage of people who aren’t very knowledgeable about scams. Scams hurt people daily which is why it’s so important to prevent users from being scammed by spreading information in an easy to understand way. The best way to avoid scams is to know about different types of scams and how they work.</p>
		</div>
	</div>
</div>

<h1>Works Cited</h1>
<hr>
<p class=p-header-left>.Zip Domains</p>
<ul>
	<li>.zip Domain Registration - .zip Domains - Register .zip (101domain.com) 101domain. .“Zip Domain Registration - .Zip Domains - Register .Zip.” 101domain, 5 June 2023, www.101domain.com/zip.htm.</li>
	<li>Bauer, Ted. “Two Faced People Shouldn’t Become Leaders.” The Context of Things, 4 May 2017, thecontextofthings.com/2017/05/04/two-faced-people.</li>
	<li>Cannot Open Zipped File? A Full Guide to Fix It! [2023] (wondershare.com) Cannot Open Zipped File? A Full Guide to Fix It! [2023]. repairit.wondershare.com/file-repair/cannot-open-zip-file.html.</li>
	<li>Computer Storage Devices. Definition | by Tharinduprabathjayapathma | Medium Tharinduprabathjayapathma. “Computer Storage Devices - Tharinduprabathjayapathma - Medium.” Medium, 5 Jan. 2022, medium.com/@tharinduprabathjayapathma/computer-storage-devices-ff64e72d964e.</li>
	<li>GeeksforGeeks. “Working of Domain Name System  DNS  Server.” GeeksforGeeks, Mar. 2023, www.geeksforgeeks.org/working-of-domain-name-system-dns-server.</li>
	<li>Get up to speed with .zip – Google Domains “Get up to Speed With .Zip – Google Domains.” Google Domains, domains.google/tld/zip.</li>
	<li>Gil, Paul. “What Are 'Zip' and 'WinZip'?” Lifewire, July 2021, www.lifewire.com/what-is-zip-and-winzip-2483210.</li>
	<li>How to Create a ZIP File on Windows, macOS, and Linux - Tech Quintal Milan. “How to Create a ZIP File on Windows, macOS, and Linux.” Tech Quintal, Jan. 2023, www.techquintal.com/create-a-zip-file.</li>
	<li>9 types of malware and how to recognize them | CSO Online Grimes, Roger A. “9 Types of Malware and How to Recognize Them.” CSO Online, 17 Nov. 2020, www.csoonline.com/article/2615925/security-your-quick-guide-to-malware-types.html.</li>
	<li>“6 Sure Signs Someone Is Phishing You—besides Email.” Malwarebytes, 20 Sept. 2018, www.malwarebytes.com/blog/news/2018/09/6-sure-signs-someone-is-phishing-you-besides-email.</li>
	<li>The Real Risks in Google’s New .Zip and .Mov Domains | WIRED Newman, Lily Hay. “The Real Risks in Google’s New .Zip and .Mov Domains.” WIRED, 21 May 2023, www.wired.com/story/google-zip-mov-domains-phishing-risks.</li>
	<li>What is a Top-Level Domain and Why it’s Important | Bobology.com bobology.com. “What Is a Top-Level Domain and Why It’s Important.” www.bobology.com, Aug. 2017, www.bobology.com/public/What-is-a-TopLevel-Domain-and-Why-its-Important.cfm.</li>
</ul>
<br>
<p class=p-header-left>Web Skimmers</p>
<ul>
	<li>Jin Chen, Tao Yan. “A Closer Look at the Web Skimmer.” Unit 42, 28 Jan. 2022, unit42.paloaltonetworks.com/web-skimmer/.</li>
	<li>Farrelly, Jessica. “High-Profile Company Data Breaches 2023.” Electric, 23 May 2023, www.electric.ai/blog/recent-big-company-data-breaches.</li>
	<li>"Web skimming." Wikipedia, The Free Encyclopedia, Wikimedia Foundation, 5 June 2023, en.wikipedia.org/wiki/Web_skimming.</li>
	<li>"eSkimming." National Initiative for Cybersecurity Careers and Studies (NICCS), CISA (Cybersecurity and Infrastructure Security Agency), 2021, niccs.cisa.gov/sites/default/files/documents/pdf/ncsam_eskimming_508.pdf.</li>
	<li>"Web skimming: Hackers infiltrate over 40 eCommerce websites (that we know of)." TechRadar, Future US, Inc., 2023, www.techradar.com/news/web-skimming-hackers-infiltrate-over-40-ecommerce-websites-that-we-know-of.</li>
</ul>



<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
