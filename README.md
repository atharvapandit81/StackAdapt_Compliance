Ad Compliance Automation for StackAdapt
Overview:

This repository contains a Python-based solution designed to automate the compliance check for ads being submitted to the StackAdapt platform. The tool was developed in response to a communication gap between the Account Executive (AE) and Platform Quality (PQ) teams at StackAdapt, which led to ads being flagged post-upload for non-compliance with platform rules and regulations.

The solution performs the following:

Image Compliance: Ensures that the ad images meet specific technical requirements such as resolution, file format, color mode, and file size.
Text Detection: Uses Google Cloud Vision to detect problematic words (like "LEGAL") in the ad images, ensuring that they do not contain non-compliant language before submission.
Customizable Framework: The code is designed to be extensible. New compliance rules (such as prohibited terms, logos, or symbols) can easily be added to the detection process, making the tool adaptable to future needs.
Use Case:

Before uploading any ad to StackAdapt, this tool can be run to ensure that the ad content is compliant with the PQ team’s guidelines. This eliminates the risk of having ads flagged post-upload, improving the approval timeline and reducing the need for constant communication between the AE and PQ teams.

Key Benefits:

Time Savings: Automates compliance checks before submission, reducing delays caused by flagged ads.
Better Communication: Streamlines the ad approval process by ensuring that both the AE and PQ teams are on the same page from the start.
Scalable & Customizable: The framework is designed to grow with the company’s changing compliance needs, making it a long-term solution.
Future Implications for StackAdapt:

Consistency Across Teams: This tool ensures consistent compliance across all ads submitted, leading to fewer disputes or rejections.
Improved Workflow: The process becomes much smoother, with reduced manual intervention and faster ad turnaround times.
Scalability: As new regulations emerge or additional compliance checks are introduced, this tool can evolve to meet those needs without needing to start from scratch.
Proactive Compliance: The tool moves from reactive to proactive compliance, ensuring that any compliance-related issues are caught before they arise, thus improving brand trust and performance on StackAdapt.
Usage Instructions:

Install required dependencies:

pip install pillow google-cloud-vision

Set up Google Cloud credentials by exporting your JSON key file:

export GOOGLE_APPLICATION_CREDENTIALS="/path/to/credentials.json"
    
Customize the code to include additional checks as needed.

