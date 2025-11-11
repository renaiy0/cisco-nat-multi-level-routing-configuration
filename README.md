<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NAT Simulation - Video Tutorial</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        header {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            margin-bottom: 30px;
            text-align: center;
        }

        h1 {
            color: #667eea;
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .subtitle {
            color: #666;
            font-size: 1.2em;
        }

        .video-section {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            margin-bottom: 30px;
        }

        .video-section h2 {
            color: #667eea;
            margin-bottom: 15px;
            font-size: 1.8em;
            border-left: 5px solid #667eea;
            padding-left: 15px;
        }

        .video-section p {
            color: #666;
            margin-bottom: 20px;
            line-height: 1.6;
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        .video-placeholder {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            color: white;
        }

        .video-placeholder svg {
            width: 80px;
            height: 80px;
            margin-bottom: 20px;
            opacity: 0.8;
        }

        .video-placeholder h3 {
            font-size: 1.5em;
            margin-bottom: 10px;
        }

        .video-placeholder p {
            color: rgba(255,255,255,0.8);
        }

        .steps-list {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
        }

        .steps-list h3 {
            color: #667eea;
            margin-bottom: 15px;
        }

        .steps-list ul {
            list-style: none;
            padding-left: 0;
        }

        .steps-list li {
            padding: 10px 0;
            padding-left: 30px;
            position: relative;
            color: #555;
        }

        .steps-list li:before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
            font-size: 1.2em;
        }

        footer {
            text-align: center;
            color: white;
            margin-top: 40px;
            padding: 20px;
        }

        footer a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        footer a:hover {
            text-decoration: underline;
        }

        .badge {
            display: inline-block;
            background: #667eea;
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9em;
            margin-right: 10px;
            margin-bottom: 10px;
        }

        .topology-image {
            width: 100%;
            border-radius: 10px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🌐 NAT Simulation Video Tutorial</h1>
            <p class="subtitle">Network Address Translation with 3 Routers - Complete Guide</p>
            <div style="margin-top: 20px;">
                <span class="badge">Cisco Packet Tracer</span>
                <span class="badge">3 Routers</span>
                <span class="badge">NAT Configuration</span>
                <span class="badge">Static Routing</span>
            </div>
        </header>

        <!-- Network Topology Overview -->
        <div class="video-section">
            <h2>📊 Network Topology</h2>
            <p>This simulation demonstrates a network with three separate subnets interconnected via routers using NAT and static routing.</p>
            <!-- Add your topology image here -->
            <img src="topology.png" alt="Network Topology" class="topology-image">
            
            <div class="steps-list">
                <h3>Network Configuration:</h3>
                <ul>
                    <li><strong>Network 1:</strong> 10.10.10.0/24 (PC0, PC1) → Router0</li>
                    <li><strong>Network 2:</strong> 20.20.20.0/24 (PC2, PC3) → Router1</li>
                    <li><strong>Network 3:</strong> 30.30.30.0/24 (PC4, PC6) → Router2</li>
                    <li><strong>Router Link 1:</strong> 40.40.40.0/24 (Router0 ↔ Router1)</li>
                    <li><strong>Router Link 2:</strong> 50.50.50.0/24 (Router1 ↔ Router2)</li>
                </ul>
            </div>
        </div>

        <!-- Video 1: Introduction -->
        <div class="video-section">
            <h2>🎬 Part 1: Introduction & Setup</h2>
            <p>Learn about the network topology and initial setup requirements for this NAT simulation project.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <!-- Example for YouTube: <iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID" allowfullscreen></iframe> -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
        </div>

        <!-- Video 2: Router Configuration -->
        <div class="video-section">
            <h2>⚙️ Part 2: Router Configuration</h2>
            <p>Step-by-step guide to configuring Router0, Router1, and Router2 with proper interfaces and IP addresses.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>What you'll learn:</h3>
                <ul>
                    <li>Configure FastEthernet and Serial interfaces</li>
                    <li>Set IP addresses for each interface</li>
                    <li>Configure clock rates on serial connections</li>
                    <li>Enable interfaces with "no shutdown" command</li>
                </ul>
            </div>
        </div>

        <!-- Video 3: NAT Configuration -->
        <div class="video-section">
            <h2>🔒 Part 3: NAT Configuration</h2>
            <p>Configure Network Address Translation (NAT) on all three routers to enable inter-network communication.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>What you'll learn:</h3>
                <ul>
                    <li>Configure NAT inside interfaces (LAN side)</li>
                    <li>Configure NAT outside interfaces (WAN side)</li>
                    <li>Set up access control lists (ACLs)</li>
                    <li>Enable NAT overload (PAT)</li>
                </ul>
            </div>
        </div>

        <!-- Video 4: Static Routing -->
        <div class="video-section">
            <h2>🛣️ Part 4: Static Routing Configuration</h2>
            <p>Configure static routes to enable communication between all three networks through the routers.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>What you'll learn:</h3>
                <ul>
                    <li>Understand routing table concepts</li>
                    <li>Add static routes using "ip route" command</li>
                    <li>Configure next-hop addresses</li>
                    <li>Verify routing with "show ip route"</li>
                </ul>
            </div>
        </div>

        <!-- Video 5: PC Configuration -->
        <div class="video-section">
            <h2>💻 Part 5: PC Configuration</h2>
            <p>Configure IP addresses, subnet masks, and default gateways on all six PCs in the network.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>What you'll learn:</h3>
                <ul>
                    <li>Configure static IP addresses on PCs</li>
                    <li>Set correct subnet masks</li>
                    <li>Configure default gateway for each network</li>
                    <li>Verify IP configuration</li>
                </ul>
            </div>
        </div>

        <!-- Video 6: Testing -->
        <div class="video-section">
            <h2>✅ Part 6: Testing & Verification</h2>
            <p>Test network connectivity and verify that NAT and routing are working correctly across all networks.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>What you'll learn:</h3>
                <ul>
                    <li>Use ping command to test connectivity</li>
                    <li>Verify NAT translations with "show ip nat translations"</li>
                    <li>Check routing tables on all routers</li>
                    <li>Troubleshoot common connectivity issues</li>
                </ul>
            </div>
        </div>

        <!-- Video 7: Troubleshooting -->
        <div class="video-section">
            <h2>🔧 Part 7: Troubleshooting Common Issues</h2>
            <p>Learn how to identify and fix common problems in NAT and routing configurations.</p>
            <div class="video-container">
                <!-- REPLACE THIS WITH YOUR VIDEO EMBED CODE -->
                <div class="video-placeholder">
                    <svg fill="white" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    <h3>Video Coming Soon</h3>
                    <p>Add your video embed code here</p>
                </div>
            </div>
            <div class="steps-list">
                <h3>Common Issues Covered:</h3>
                <ul>
                    <li>Interfaces showing "down" status</li>
                    <li>Incorrect gateway configuration</li>
                    <li>NAT not translating addresses</li>
                    <li>Routing loops or missing routes</li>
                    <li>Serial connection clock rate issues</li>
                </ul>
            </div>
        </div>

        <footer>
            <p>📚 For detailed written instructions, check the <a href="README.md">README.md</a> file</p>
            <p style="margin-top: 10px;">🎓 Created for educational purposes - Cisco Packet Tracer Simulation</p>
        </footer>
    </div>
</body>
</html>
