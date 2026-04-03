[Uploading Htet_Thura_Oo_CV_Enhanced.html…]()
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Htet Thura Oo - CV</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #0f172a 100%);
            color: #1e293b;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        .cv-wrapper {
            display: grid;
            grid-template-columns: 300px 1fr;
            gap: 30px;
            background: white;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
        }

        /* LEFT SIDEBAR */
        .sidebar {
            background: linear-gradient(180deg, #1e293b 0%, #0f172a 100%);
            padding: 40px 30px;
            position: relative;
            overflow: hidden;
        }

        .sidebar::before {
            content: '';
            position: absolute;
            inset: 0;
            background-image: 
                radial-gradient(circle at 20% 50%, rgba(6, 182, 212, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(2, 132, 199, 0.1) 0%, transparent 50%);
            pointer-events: none;
        }

        .header-bar {
            background: linear-gradient(135deg, #06b6d4 0%, #0284c7 100%);
            padding: 25px;
            border-radius: 12px;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
        }

        .header-bar::before {
            content: '';
            position: absolute;
            inset: 0;
            background-image: 
                linear-gradient(45deg, transparent 30%, rgba(255,255,255,0.1) 50%, transparent 70%);
            background-size: 20px 20px;
            opacity: 0.3;
        }

        .header-bar h1 {
            font-size: 28px;
            font-weight: 900;
            color: white;
            line-height: 1.2;
            position: relative;
            z-index: 1;
            letter-spacing: -1px;
        }

        .header-bar .subtitle {
            color: #cffafe;
            font-size: 12px;
            font-weight: 600;
            margin-top: 10px;
            display: flex;
            align-items: center;
            position: relative;
            z-index: 1;
        }

        .header-bar .subtitle::before {
            content: '';
            display: inline-block;
            width: 6px;
            height: 6px;
            background: #a5f3fc;
            border-radius: 50%;
            margin-right: 8px;
        }

        .sidebar-section {
            margin-bottom: 30px;
            position: relative;
            z-index: 2;
        }

        .sidebar-section h3 {
            color: #06b6d4;
            font-size: 12px;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }

        .sidebar-section h3::before {
            content: '';
            display: inline-block;
            width: 6px;
            height: 6px;
            background: #06b6d4;
            border-radius: 50%;
            margin-right: 10px;
        }

        .contact-item {
            margin-bottom: 12px;
        }

        .contact-label {
            color: #94a3b8;
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 4px;
            font-weight: 600;
        }

        .contact-value {
            color: white;
            font-size: 13px;
            font-weight: 500;
        }

        .contact-value a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .contact-value a:hover {
            color: #06b6d4;
        }

        .skill-tag {
            display: inline-block;
            padding: 6px 12px;
            background: rgba(6, 182, 212, 0.2);
            border: 1px solid rgba(6, 182, 212, 0.5);
            color: #06b6d4;
            font-size: 11px;
            border-radius: 20px;
            font-weight: 500;
            margin-right: 6px;
            margin-bottom: 6px;
        }

        .cert-item {
            margin-bottom: 12px;
            display: flex;
            align-items: flex-start;
        }

        .cert-item::before {
            content: '▸';
            color: #06b6d4;
            margin-right: 10px;
            font-weight: bold;
            margin-top: 2px;
        }

        .cert-name {
            color: white;
            font-weight: 600;
            font-size: 13px;
        }

        .cert-desc {
            color: #94a3b8;
            font-size: 11px;
            margin-top: 2px;
        }

        /* MAIN CONTENT */
        .main-content {
            padding: 40px;
            background: white;
        }

        .content-section {
            margin-bottom: 35px;
        }

        .content-section h2 {
            font-size: 20px;
            font-weight: 900;
            color: #0f172a;
            text-transform: uppercase;
            letter-spacing: -0.5px;
            margin-bottom: 20px;
            padding-bottom: 12px;
            border-left: 4px solid #06b6d4;
            padding-left: 15px;
        }

        .summary-text {
            color: #475569;
            line-height: 1.7;
            font-size: 14px;
        }

        .education-item {
            display: flex;
            gap: 20px;
        }

        .icon-box {
            flex-shrink: 0;
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, #0284c7 0%, #06b6d4 100%);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }

        .education-content h3 {
            font-size: 16px;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 5px;
        }

        .education-content p {
            color: #64748b;
            font-size: 13px;
        }

        .experience-item {
            display: flex;
            gap: 20px;
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 2px solid #e2e8f0;
        }

        .experience-item:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }

        .experience-content h3 {
            font-size: 16px;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 5px;
        }

        .experience-role {
            color: #06b6d4;
            font-weight: 600;
            font-size: 13px;
            margin-bottom: 10px;
        }

        .experience-desc {
            color: #475569;
            font-size: 13px;
            line-height: 1.6;
        }

        .roles-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
        }

        .role-card {
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            padding: 15px;
            border-radius: 8px;
            border: 1px solid #bae6fd;
        }

        .role-label {
            color: #0284c7;
            font-size: 11px;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 8px;
        }

        .role-title {
            color: #0f172a;
            font-weight: 700;
            font-size: 14px;
            margin-bottom: 8px;
        }

        .role-desc {
            color: #475569;
            font-size: 12px;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
        }

        .project-card {
            background: linear-gradient(135deg, #06b6d4 0%, #0284c7 100%);
            padding: 20px;
            border-radius: 8px;
            color: white;
        }

        .project-icon {
            font-size: 32px;
            margin-bottom: 10px;
        }

        .project-title {
            font-weight: 700;
            font-size: 14px;
            margin-bottom: 8px;
        }

        .project-desc {
            font-size: 12px;
            color: rgba(255, 255, 255, 0.9);
            line-height: 1.5;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .skill-category h3 {
            color: #0f172a;
            font-weight: 700;
            font-size: 14px;
            margin-bottom: 12px;
            display: flex;
            align-items: center;
        }

        .skill-category h3::before {
            content: '';
            display: inline-block;
            width: 6px;
            height: 6px;
            background: #06b6d4;
            border-radius: 50%;
            margin-right: 10px;
        }

        .skill-item {
            color: #475569;
            font-size: 13px;
            margin-bottom: 8px;
        }

        .skill-item::before {
            content: '✓ ';
            color: #06b6d4;
            font-weight: bold;
            margin-right: 6px;
        }

        .footer {
            text-align: center;
            padding-top: 20px;
            color: #94a3b8;
            font-size: 12px;
            border-top: 1px solid #e2e8f0;
        }

        @media (max-width: 768px) {
            .cv-wrapper {
                grid-template-columns: 1fr;
            }

            .roles-grid {
                grid-template-columns: 1fr;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }
        }

        @media print {
            body {
                background: white;
            }

            .cv-wrapper {
                box-shadow: none;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="cv-wrapper">
            <!-- LEFT SIDEBAR -->
            <div class="sidebar">
                <div class="header-bar">
                    <h1>HTET<br>THURA<br>OO</h1>
                    <div class="subtitle">IT Professional</div>
                </div>

                <!-- Contact Section -->
                <div class="sidebar-section">
                    <h3>Contact</h3>
                    <div class="contact-item">
                        <div class="contact-label">Phone</div>
                        <div class="contact-value"><a href="tel:09770025700">09770025700</a></div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-label">Email</div>
                        <div class="contact-value"><a href="mailto:thura8385@gmail.com">thura8385@gmail.com</a></div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-label">Location</div>
                        <div class="contact-value">Hlaing Township, Yangon</div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-label">DOB</div>
                        <div class="contact-value">26.05.1999</div>
                    </div>
                </div>

                <!-- Links Section -->
                <div class="sidebar-section">
                    <h3>Links</h3>
                    <div class="contact-item">
                        <div class="contact-value"><a href="https://www.facebook.com/share/1HY4GRXQtQ/?mibextid=wwXIfr" target="_blank">→ Facebook Profile</a></div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-value"><a href="https://htetfolio-7g25hgwh.manus.space" target="_blank">→ Portfolio Website</a></div>
                    </div>
                </div>

                <!-- Technical Skills -->
                <div class="sidebar-section">
                    <h3>Technical Skills</h3>
                    <div>
                        <div class="contact-label" style="margin-bottom: 8px;">Laptops & Mobile</div>
                        <div>
                            <span class="skill-tag">Hardware</span>
                            <span class="skill-tag">Software</span>
                        </div>
                    </div>
                    <div style="margin-top: 12px;">
                        <div class="contact-label" style="margin-bottom: 8px;">Operating Systems</div>
                        <div>
                            <span class="skill-tag">All OS</span>
                        </div>
                    </div>
                </div>

                <!-- Certifications -->
                <div class="sidebar-section">
                    <h3>Certifications</h3>
                    <div class="cert-item">
                        <div>
                            <div class="cert-name">CompTIA A+</div>
                            <div class="cert-desc">IT Certification</div>
                        </div>
                    </div>
                    <div class="cert-item">
                        <div>
                            <div class="cert-name">Networking</div>
                            <div class="cert-desc">Professional Training</div>
                        </div>
                    </div>
                    <div class="cert-item">
                        <div>
                            <div class="cert-name">Mobile Service</div>
                            <div class="cert-desc">Technical Training</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- MAIN CONTENT -->
            <div class="main-content">
                <!-- Professional Summary -->
                <div class="content-section">
                    <h2>Professional Summary</h2>
                    <p class="summary-text">
                        Highly motivated and versatile IT professional with comprehensive experience in technical support, customer service, and AI coaching. Possesses strong technical expertise in laptop and mobile hardware/software maintenance, combined with effective communication abilities. Committed to delivering exceptional technical solutions and driving digital transformation initiatives.
                    </p>
                </div>

                <!-- Education -->
                <div class="content-section">
                    <h2>Education</h2>
                    <div class="education-item">
                        <div class="icon-box">📚</div>
                        <div class="education-content">
                            <h3>B.Sc Chemistry</h3>
                            <p>Scientific foundation with analytical and research capabilities</p>
                        </div>
                    </div>
                </div>

                <!-- Work Experience -->
                <div class="content-section">
                    <h2>Work Experience</h2>
                    <div class="experience-item">
                        <div class="icon-box" style="background: linear-gradient(135deg, #06b6d4 0%, #0284c7 100%);">📱</div>
                        <div class="experience-content">
                            <h3>Power Mobile Center</h3>
                            <div class="experience-role">Mobile Technician | 1 Year 6 Months</div>
                            <p class="experience-desc">Provided comprehensive mobile device repair and maintenance services. Diagnosed hardware and software issues, performed technical troubleshooting, and delivered exceptional customer support for mobile devices and accessories.</p>
                        </div>
                    </div>
                    <div class="experience-item">
                        <div class="icon-box" style="background: linear-gradient(135deg, #0284c7 0%, #1e3a8a 100%);">💻</div>
                        <div class="experience-content">
                            <h3>UNiQUE IT & Electronics</h3>
                            <div class="experience-role">Customer Support - Service Technician</div>
                            <p class="experience-desc">Delivered technical assistance and support for IT and electronic products. Performed advanced troubleshooting and repairs on computer systems and peripherals while maintaining high levels of customer satisfaction and service quality.</p>
                        </div>
                    </div>
                </div>

                <!-- Professional Roles -->
                <div class="content-section">
                    <h2>Professional Roles</h2>
                    <div class="roles-grid">
                        <div class="role-card">
                            <div class="role-label">Role 01</div>
                            <div class="role-title">IT Supporter</div>
                            <div class="role-desc">Technical support and system administration</div>
                        </div>
                        <div class="role-card">
                            <div class="role-label">Role 02</div>
                            <div class="role-title">AI Coaching</div>
                            <div class="role-desc">AI technology training and guidance</div>
                        </div>
                        <div class="role-card">
                            <div class="role-label">Role 03</div>
                            <div class="role-title">Communication</div>
                            <div class="role-desc">Client relations and service delivery</div>
                        </div>
                    </div>
                </div>

                <!-- Projects & Highlights -->
                <div class="content-section">
                    <h2>Projects & Highlights</h2>
                    <div class="projects-grid">
                        <div class="project-card">
                            <div class="project-icon">📱</div>
                            <div class="project-title">Mobile Service Training</div>
                            <div class="project-desc">Comprehensive mobile device maintenance and repair expertise</div>
                        </div>
                        <div class="project-card" style="background: linear-gradient(135deg, #0284c7 0%, #1e3a8a 100%);">
                            <div class="project-icon">🤖</div>
                            <div class="project-title">AI Projects</div>
                            <div class="project-desc">Implementation and coaching in artificial intelligence technologies</div>
                        </div>
                        <div class="project-card" style="background: linear-gradient(135deg, #1e3a8a 0%, #06b6d4 100%);">
                            <div class="project-icon">🎬</div>
                            <div class="project-title">Video Editing</div>
                            <div class="project-desc">Professional video production and content creation</div>
                        </div>
                        <div class="project-card" style="background: linear-gradient(135deg, #06b6d4 0%, #0284c7 100%);">
                            <div class="project-icon">📹</div>
                            <div class="project-title">Mobile Review Videos</div>
                            <div class="project-desc">Technical review and demonstration content creation</div>
                        </div>
                    </div>
                </div>

                <!-- Digital Skills -->
                <div class="content-section">
                    <h2>Digital Skills</h2>
                    <div class="skills-grid">
                        <div>
                            <h3>Technical Expertise</h3>
                            <div class="skill-item">Laptop & Mobile Hardware</div>
                            <div class="skill-item">Software Troubleshooting</div>
                            <div class="skill-item">Operating System Management</div>
                            <div class="skill-item">Network Configuration</div>
                        </div>
                        <div>
                            <h3>Digital Services</h3>
                            <div class="skill-item">Social Media Management</div>
                            <div class="skill-item">Content Boosting Services</div>
                            <div class="skill-item">Video Editing & Production</div>
                            <div class="skill-item">Customer Support</div>
                        </div>
                    </div>
                </div>

                <div class="footer">
                    <p>© 2026 Htet Thura Oo | IT Professional | All Rights Reserved</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
