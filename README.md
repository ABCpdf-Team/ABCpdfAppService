<h1>ABCpdfAppService</h1>
<h3>.NET 5 Azure App Service demonstrating HTML to PDF conversion using <a href="https://www.websupergoo.com/abcpdf-1.aspx">ABCpdf</a>.</h3>
<p>This is an example solution for performing HTML to PDF conversion in a .NET 5 Azure App Service using using ABCpdf's <a href="https://www.websupergoo.com/helppdfnet/default.htm?page=source%2F5-abcpdf%2Fxhtmloptions%2F2-properties%2Ffireshield.htm">
ABCWebKit engine</a>.</p>
<p>Follow these steps to get your App Service up and running:</p>
<ul>
<li>Clone the project.</li>
<li>Ensure that the <a href="https://www.nuget.org/packages/ABCpdf/">ABCpdf</a> and <a href="">ABCpdf.ABCWebKit</a> NuGet packages are restored/installed.</li>
<li>Copy your ABCpdf license key where specified in Startup.cs.</li>
<li>Build and test locally.</li>
<li>Create a Windows .NET 5 Web App in your Azure portal.</li>
<li><strong>NB the minimum App Service plan the ABCWEbkit will work on is a Basic B1 instance.</strong> This is Microsft's policy and may incur charges even for development.</li>
<li><strong>Change the App Service platform to "64 Bit"</strong> in the App Service Configuration/General Settings. <strong>It will not work on a 32-bit platform!</strong></li> 
<li>Publish the solution to the Azure App Service <strong>ensuring your target runtime is "win-x64"</strong>.</li>
</ul>
<p>The ABCWebKit engine has been built on <a href="https://wkhtmltopdf.org/">wkhtmltopdf</a> which in turn is based on a version of QTWebKit 
from 2012 which was last updated in 2015! Therefore <strong><em>we strongly recommend that you only use the ABCWebkit engine to process HTML that you trust</em></strong>.</p>
<p>More information may be gleaned from our <a href="https://www.websupergoo.com/support-azure-abcpdf.aspx">Azure Deployment Guide</a>.</p>
<p>This solution was last tested in March 2021. Do bear in mind how often the Azure framework changes when following these instructions, especially in terms of nomenclature!</p>
<p>ABCpdf has extensive documentation and examples <a href="https://www.websupergoo.com/helppdfnet/default.htm">online</a> and in the <a href="https://www.websupergoo.com/abcpdf-download.aspx">full ABCpdf installer package</a>.</p>
<em>The ABCpdf Team</em>