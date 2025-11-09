<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pravin A - VLSI Design Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --success: #2ecc71;
            --warning: #f39c12;
            --gray: #95a5a6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 40px 20px;
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .profile-header {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 30px;
        }
        
        .profile-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            background-color: var(--light);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: var(--primary);
            border: 5px solid white;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
        }
        
        .profile-info {
            flex: 1;
            min-width: 300px;
        }
        
        .profile-info h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .profile-info h2 {
            font-size: 1.2rem;
            font-weight: 400;
            margin-bottom: 15px;
            opacity: 0.9;
        }
        
        .profile-info p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .badge {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin-right: 10px;
            margin-bottom: 10px;
        }
        
        .section {
            background: white;
            border-radius: 10px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .section-title {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--light);
        }
        
        .section-title i {
            color: var(--secondary);
            font-size: 1.5rem;
        }
        
        .section-title h2 {
            font-size: 1.8rem;
            color: var(--primary);
        }
        
        .card-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .card {
            background: var(--light);
            border-radius: 8px;
            padding: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border-left: 4px solid var(--secondary);
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .card h3 {
            color: var(--primary);
            margin-bottom: 10px;
            font-size: 1.3rem;
        }
        
        .card p {
            color: #555;
            margin-bottom: 15px;
        }
        
        .card .date {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .skill-category {
            flex: 1;
            min-width: 250px;
        }
        
        .skill-category h3 {
            margin-bottom: 15px;
            color: var(--primary);
            padding-bottom: 5px;
            border-bottom: 1px solid var(--light);
        }
        
        .skill-item {
            margin-bottom: 10px;
        }
        
        .skill-name {
            display: flex;
            justify-content: space-between;
            margin-bottom: 5px;
        }
        
        .skill-bar {
            height: 8px;
            background-color: #e0e0e0;
            border-radius: 4px;
            overflow: hidden;
        }
        
        .skill-level {
            height: 100%;
            background-color: var(--secondary);
            border-radius: 4px;
        }
        
        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }
        
        .contact-btn {
            display: flex;
            align-items: center;
            gap: 10px;
            background: var(--primary);
            color: white;
            padding: 12px 20px;
            border-radius: 5px;
            text-decoration: none;
            transition: background 0.3s ease;
        }
        
        .contact-btn:hover {
            background: var(--secondary);
        }
        
        .nav-tabs {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 30px;
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .nav-tab {
            padding: 10px 20px;
            background: var(--light);
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .nav-tab.active {
            background: var(--secondary);
            color: white;
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
        }
        
        .achievement-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .achievement-card {
            background: var(--light);
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .achievement-card:hover {
            transform: scale(1.05);
        }
        
        .achievement-card i {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 15px;
        }
        
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .timeline::after {
            content: '';
            position: absolute;
            width: 4px;
            background-color: var(--light);
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -2px;
        }
        
        .timeline-item {
            padding: 10px 40px;
            position: relative;
            width: 50%;
            box-sizing: border-box;
        }
        
        .timeline-item::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: white;
            border: 4px solid var(--secondary);
            border-radius: 50%;
            top: 15px;
            right: -10px;
            z-index: 1;
        }
        
        .left {
            left: 0;
        }
        
        .right {
            left: 50%;
        }
        
        .right::after {
            left: -10px;
        }
        
        .timeline-content {
            padding: 20px;
            background-color: white;
            border-radius: 6px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }
        
        footer {
            text-align: center;
            padding: 30px 0;
            color: var(--gray);
            border-top: 1px solid var(--light);
            margin-top: 50px;
        }
        
        @media (max-width: 768px) {
            .timeline::after {
                left: 31px;
            }
            
            .timeline-item {
                width: 100%;
                padding-left: 70px;
                padding-right: 25px;
            }
            
            .timeline-item::after {
                left: 21px;
            }
            
            .right {
                left: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile-header">
                <div class="profile-image">
                    <i class="fas fa-user"></i>
                </div>
                <div class="profile-info">
                    <h1>Pravin A</h1>
                    <h2>VLSI Design | Circuit Design | RTL Design | Verilog</h2>
                    <p><i class="fas fa-map-marker-alt"></i> Namakkal, Tamil Nadu, India</p>
                    <p><i class="fas fa-briefcase"></i> FOSSEE Intern @ IIT Bombay (Remote)</p>
                    <p><i class="fas fa-graduation-cap"></i> B.E. Electronics and Communication Engineering</p>
                    <div>
                        <span class="badge">VLSI Design</span>
                        <span class="badge">Circuit Design</span>
                        <span class="badge">RTL Design</span>
                        <span class="badge">Verilog</span>
                    </div>
                </div>
            </div>
        </header>
        
        <div class="nav-tabs">
            <div class="nav-tab active" data-tab="about">About</div>
            <div class="nav-tab" data-tab="experience">Experience</div>
            <div class="nav-tab" data-tab="education">Education</div>
            <div class="nav-tab" data-tab="projects">Projects</div>
            <div class="nav-tab" data-tab="skills">Skills</div>
            <div class="nav-tab" data-tab="achievements">Achievements</div>
            <div class="nav-tab" data-tab="contact">Contact</div>
        </div>
        
        <div class="tab-content active" id="about">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-user-tie"></i>
                    <h2>Career Objective</h2>
                </div>
                <p>Aspiring professional in the semiconductor industry, currently pursuing a Bachelor's degree in Electronics and Communication Engineering. Passionate about VLSI design, digital IC development, and semiconductor devices, with strong fundamentals in digital logic, circuit simulation, and hardware description languages (Verilog).</p>
                <p>Dedicated to exploring the end-to-end chip design flow — from device physics and circuit analysis to FPGA prototyping and system-level integration. Aiming to contribute to innovations in semiconductor and VLSI technologies, including digital IC design, embedded systems, and next-generation chip technologies.</p>
            </div>
        </div>
        
        <div class="tab-content" id="experience">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-briefcase"></i>
                    <h2>Work Experience</h2>
                </div>
                <div class="card">
                    <h3>FOSSEE, IIT Bombay</h3>
                    <p class="date">Oct 2025 – Present</p>
                    <p><strong>Role:</strong> Research Migration Contributor | Analog Circuit Design</p>
                    <h4>Key Contributions:</h4>
                    <ul>
                        <li>Migrated and simulated analog signal circuits under the FOSSEE eSim initiative, focusing on CMOS-based charge pump designs.</li>
                        <li>Enhanced knowledge of open-source EDA tools such as KiCad and Ngspice.</li>
                        <li>Completed and documented three major projects:
                            <ul>
                                <li>DC–DC Voltage Multiplier using Dickson Charge Pump Topology</li>
                                <li>Design and Simulation of a Low-Voltage Cross-Coupled Charge Pump</li>
                                <li>Six-Stage Linear CMOS Charge Pump with Complementary Clocking</li>
                            </ul>
                        </li>
                        <li>Strengthened understanding of analog system modeling, charge transfer mechanisms, and low-voltage CMOS circuits.</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="tab-content" id="education">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-graduation-cap"></i>
                    <h2>Education</h2>
                </div>
                <div class="timeline">
                    <div class="timeline-item left">
                        <div class="timeline-content">
                            <h3>Bachelor of Engineering (B.E.)</h3>
                            <p>Electronics and Communication Engineering</p>
                            <p>Sri Eshwar College of Engineering, Coimbatore</p>
                            <p class="date">Aug 2024 – Jul 2028</p>
                        </div>
                    </div>
                    <div class="timeline-item right">
                        <div class="timeline-content">
                            <h3>Higher Secondary Education</h3>
                            <p>Mathematics & Computer Science</p>
                            <p>Holy Angel's Matric Higher Secondary School</p>
                            <p class="date">Jun 2023 – Mar 2024 | Grade: 95%</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="tab-content" id="projects">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-project-diagram"></i>
                    <h2>Projects & Research</h2>
                </div>
                <div class="card-container">
                    <div class="card">
                        <h3>Electronic Voting System</h3>
                        <p>Designed and simulated during a VLSI Hackathon using Xilinx Vivado. Implemented complete system using Verilog modules for real-time voting simulation.</p>
                        <p><strong>Tools:</strong> Xilinx Vivado, Verilog, GitHub</p>
                    </div>
                    <div class="card">
                        <h3>Analog Design using Cadence Virtuoso</h3>
                        <p>Designed and analyzed Common Emitter (CE) Amplifier. Performed DC and transient analyses to evaluate amplifier characteristics.</p>
                        <p><strong>Tools:</strong> Cadence Virtuoso</p>
                    </div>
                    <div class="card">
                        <h3>Adaptive Vision - Smart Lighting System</h3>
                        <p>IoT + AI project developed for SelfE Hackathon'24. Integrated motion sensors and rain detection for adaptive light control. Secured Special Prize among 30 teams.</p>
                        <p><strong>Technologies:</strong> IoT, AI, Sensors</p>
                    </div>
                    <div class="card">
                        <h3>Research Migration Projects</h3>
                        <p>Focused on CMOS charge pump simulations using open-source EDA tools. Published contributions available under NMEICT – eSim Repository.</p>
                        <p><strong>Tools:</strong> eSim, KiCad, Ngspice</p>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="tab-content" id="skills">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-tools"></i>
                    <h2>Skills</h2>
                </div>
                <div class="skills-container">
                    <div class="skill-category">
                        <h3>Technical Skills</h3>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>VLSI & Design Tools</span>
                                <span>90%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 90%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Programming Languages</span>
                                <span>85%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 85%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>EDA & Simulation</span>
                                <span>88%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 88%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Hardware Tools</span>
                                <span>80%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 80%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="skill-category">
                        <h3>Soft Skills</h3>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Team Collaboration</span>
                                <span>95%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 95%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Problem Solving & Debugging</span>
                                <span>90%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 90%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Technical Documentation</span>
                                <span>85%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 85%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>Leadership & Presentation</span>
                                <span>88%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 88%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="tab-content" id="achievements">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-trophy"></i>
                    <h2>Achievements & Certifications</h2>
                </div>
                <div class="achievement-grid">
                    <div class="achievement-card">
                        <i class="fas fa-certificate"></i>
                        <h3>FOSSEE Internship</h3>
                        <p>IIT Bombay (eSim Initiative) – 2025</p>
                    </div>
                    <div class="achievement-card">
                        <i class="fas fa-award"></i>
                        <h3>Special Prize</h3>
                        <p>SelfE Hackathon 2024</p>
                    </div>
                    <div class="achievement-card">
                        <i class="fas fa-medal"></i>
                        <h3>Top 3rd Performer</h3>
                        <p>Skillrack Platform – 2024–2025</p>
                    </div>
                    <div class="achievement-card">
                        <i class="fas fa-code"></i>
                        <h3>CodeChef Gold Streak</h3>
                        <p>50-day coding streak</p>
                    </div>
                </div>
                
                <div class="section-title" style="margin-top: 40px;">
                    <i class="fas fa-certificate"></i>
                    <h2>Certifications</h2>
                </div>
                <div class="card">
                    <ul>
                        <li>Research Migration Project – DC–DC Voltage Multiplier Using Dickson Charge Pump Topology (FOSSEE, IIT Bombay) - Oct 2025</li>
                        <li>Research Migration Project – Low-Voltage Cross-Coupled Charge Pump (FOSSEE, IIT Bombay) - Oct 2025</li>
                        <li>Research Migration Project – Six-Stage Linear CMOS Charge Pump (FOSSEE, IIT Bombay) - Oct 2025</li>
                        <li>Python Programming Masterclass (Udemy) - Jul 2025</li>
                        <li>Mastering Data Structures & Algorithms using C/C++ (Udemy) - May 2025</li>
                        <li>C++ Essentials – Certificate of Excellence (Scaler) - Feb 2025</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="tab-content" id="contact">
            <div class="section">
                <div class="section-title">
                    <i class="fas fa-envelope"></i>
                    <h2>Contact Information</h2>
                </div>
                <div class="card">
                    <p><i class="fas fa-envelope"></i> <strong>Email:</strong> pravin.a2024ece@sece.ac.in</p>
                    <p><i class="fas fa-phone"></i> <strong>Phone:</strong> +91 9345802099</p>
                    <p><i class="fas fa-map-marker-alt"></i> <strong>Location:</strong> Namakkal, Tamil Nadu, India</p>
                    <p><i class="fas fa-language"></i> <strong>Languages:</strong> English, Tamil</p>
                    
                    <div class="contact-links">
                        <a href="https://github.com/pravin2007-ctrl" class="contact-btn" target="_blank">
                            <i class="fab fa-github"></i> GitHub
                        </a>
                        <a href="mailto:pravin.a2024ece@sece.ac.in" class="contact-btn">
                            <i class="fas fa-envelope"></i> Email
                        </a>
                        <a href="tel:+919345802099" class="contact-btn">
                            <i class="fas fa-phone"></i> Call
                        </a>
                    </div>
                </div>
            </div>
        </div>
        
        <footer>
            <p>&copy; 2025 Pravin A. All Rights Reserved.</p>
            <p>VLSI Design | Circuit Design | RTL Design | Verilog</p>
        </footer>
    </div>

    <script>
        // Tab navigation
        document.querySelectorAll('.nav-tab').forEach(tab => {
            tab.addEventListener('click', () => {
                // Remove active class from all tabs and contents
                document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
                document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
                
                // Add active class to clicked tab and corresponding content
                tab.classList.add('active');
                document.getElementById(tab.dataset.tab).classList.add('active');
            });
        });
    </script>
</body>
</html>
