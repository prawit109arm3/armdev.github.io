<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP Website Project Proposal Infographic</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Sarabun', sans-serif; background-color: #f8fafc; color: #1e293b; }
        .chart-container { 
            position: relative; 
            width: 100%; 
            max-width: 600px; 
            margin: 0 auto; 
            height: 350px; 
            max-height: 400px; 
        }
        @media (max-width: 640px) {
            .chart-container { height: 300px; }
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
    </style>
    <!-- 
        NARRATIVE PLAN:
        1. Header: Establish authority and project title.
        2. Introduction: Executive summary emphasizing the "Digital Infrastructure".
        3. Strategic Objectives: 4 Pillars of the project (Official, Hub, Trust, Legal) using CSS Cards.
        4. Technical Analysis (Radar Chart): Visualizing the balance of features (Security, SEO, Speed, etc.).
        5. Execution Roadmap (Timeline): Detailed breakdown of the 6 phases over 30-45 days using a CSS Timeline.
        6. Budget Allocation (Doughnut Chart): Visualizing the investment breakdown.
        7. Conclusion: Final call to action and summary.

        CHART SELECTION & NO SVG CONFIRMATION:
        1. Radar Chart (Chart.js): Selected to show the multi-faceted strengths of the proposed solution (Security vs Design vs SEO). NO SVG used.
        2. Doughnut Chart (Chart.js): Selected to show part-to-whole relationship of the budget. NO SVG used.
        3. Timeline & Flow: Implemented using Tailwind Grid/Flex and Border styling. NO SVG, NO Mermaid JS used.
        4. Icons: Standard Unicode Emojis used throughout. NO SVG icons used.
        
        PALETTE: "Vibrant Trust" - Deep Blue (#1e3a8a) for authority, Cyan (#06b6d4) for modern tech, Amber (#f59e0b) for highlights.
    -->
</head>
<body class="bg-slate-50">

    <!-- Hero Section -->
    <header class="bg-gradient-to-r from-blue-900 to-cyan-700 text-white shadow-lg">
        <div class="container mx-auto px-4 py-12 text-center">
            <h1 class="text-3xl md:text-5xl font-extrabold mb-4 leading-tight">โครงการเว็บไซต์ผู้สมัคร สส.</h1>
            <p class="text-xl md:text-2xl font-light opacity-90 mb-6">สร้างฐานที่มั่นดิจิทัล: เชื่อมต่อ ประชาชน ด้วยความน่าเชื่อถือ</p>
            <div class="inline-block bg-white text-blue-900 px-6 py-2 rounded-full font-bold shadow-md">
                Project Proposal Overview
            </div>
        </div>
    </header>

    <main class="container mx-auto px-4 py-8 space-y-12">

        <!-- Section 1: Executive Summary -->
        <section class="max-w-4xl mx-auto text-center">
            <div class="glass-card p-8 rounded-2xl shadow-xl">
                <h2 class="text-3xl font-bold text-blue-900 mb-6">บทสรุปผู้บริหาร</h2>
                <p class="text-lg text-gray-700 leading-relaxed">
                    เป้าหมายหลักของโครงการนี้คือการสร้าง <span class="font-bold text-cyan-600">"Official Digital Infrastructure"</span> 
                    (โครงสร้างพื้นฐานดิจิทัลอย่างเป็นทางการ) เพื่อเป็นศูนย์กลางข้อมูลที่ถูกต้อง รวดเร็ว และปลอดภัย 
                    ภายใต้กรอบกฎหมายการเลือกตั้ง พัฒนาด้วยระบบ WordPress มาตรฐานสากล เพื่อภาพลักษณ์ที่ยั่งยืน
                </p>
            </div>
        </section>

        <!-- Section 2: Strategic Objectives (CSS Grid - Goal: Inform) -->
        <section>
            <div class="flex items-center mb-8">
                <div class="h-10 w-2 bg-blue-600 mr-4 rounded-full"></div>
                <h2 class="text-3xl font-bold text-gray-800">วัตถุประสงค์หลัก (Strategic Objectives)</h2>
            </div>
            <p class="mb-6 text-gray-600">รากฐานสำคัญ 4 ประการที่เว็บไซต์นี้จะมอบให้กับผู้สมัคร เพื่อสร้างความได้เปรียบในการสื่อสาร</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Obj 1 -->
                <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-shadow border-t-4 border-blue-600">
                    <div class="text-4xl mb-4">🏛️</div>
                    <h3 class="text-xl font-bold mb-2">Official Presence</h3>
                    <p class="text-gray-600 text-sm">สร้างตัวตนอย่างเป็นทางการ มีความน่าเชื่อถือและเป็นมืออาชีพ</p>
                </div>
                <!-- Obj 2 -->
                <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-shadow border-t-4 border-cyan-500">
                    <div class="text-4xl mb-4">📡</div>
                    <h3 class="text-xl font-bold mb-2">Information Hub</h3>
                    <p class="text-gray-600 text-sm">ศูนย์กลางข้อมูล นโยบาย และข่าวสารที่ถูกต้องที่สุด</p>
                </div>
                <!-- Obj 3 -->
                <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-shadow border-t-4 border-amber-500">
                    <div class="text-4xl mb-4">🤝</div>
                    <h3 class="text-xl font-bold mb-2">Trust & Access</h3>
                    <p class="text-gray-600 text-sm">เข้าถึงง่ายผ่านมือถือ (Mobile Responsive) และปลอดภัย</p>
                </div>
                <!-- Obj 4 -->
                <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-shadow border-t-4 border-emerald-500">
                    <div class="text-4xl mb-4">⚖️</div>
                    <h3 class="text-xl font-bold mb-2">Legal Compliance</h3>
                    <p class="text-gray-600 text-sm">ถูกต้องตามกฎระเบียบ กกต. และกฎหมายเลือกตั้ง</p>
                </div>
            </div>
        </section>

        <!-- Section 3: Technical Standards (Chart.js Radar - Goal: Relationships/Performance) -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center bg-white rounded-3xl p-8 shadow-lg">
            <div class="order-2 md:order-1">
                <div class="flex items-center mb-6">
                    <div class="h-10 w-2 bg-cyan-500 mr-4 rounded-full"></div>
                    <h2 class="text-3xl font-bold text-gray-800">มาตรฐานทางเทคนิค</h2>
                </div>
                <p class="mb-6 text-gray-600">
                    เราให้ความสำคัญกับสมดุลของประสิทธิภาพเว็บไซต์ แผนภาพเรดาร์ด้านขวานี้แสดงให้เห็นว่าเราจัดสรรทรัพยากรและความสำคัญให้กับด้านต่างๆ อย่างไร เพื่อให้ได้เว็บไซต์ที่มีคุณภาพสูงสุด
                </p>
                <ul class="space-y-4">
                    <li class="flex items-start">
                        <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-xs font-bold mr-3 mt-1">SECURITY</span>
                        <span class="text-gray-700">ติดตั้ง SSL และระบบป้องกันการโจมตี (Firewall) เพื่อความปลอดภัยสูงสุด</span>
                    </li>
                    <li class="flex items-start">
                        <span class="bg-cyan-100 text-cyan-800 px-2 py-1 rounded text-xs font-bold mr-3 mt-1">SEO</span>
                        <span class="text-gray-700">ปรับโครงสร้าง URL และเนื้อหาให้ค้นหาเจอบน Google ได้ง่าย</span>
                    </li>
                    <li class="flex items-start">
                        <span class="bg-amber-100 text-amber-800 px-2 py-1 rounded text-xs font-bold mr-3 mt-1">MOBILE</span>
                        <span class="text-gray-700">รองรับการแสดงผลทุกอุปกรณ์ (Responsive Design) อย่างสมบูรณ์</span>
                    </li>
                </ul>
            </div>
            
            <div class="order-1 md:order-2 flex flex-col items-center justify-center">
                <h3 class="text-lg font-bold text-gray-500 mb-4 tracking-widest uppercase">Performance Metrics</h3>
                <div class="chart-container">
                    <canvas id="techRadarChart"></canvas>
                </div>
            </div>
        </section>

        <!-- Section 4: Timeline & Phases (CSS Timeline - Goal: Change/Process) -->
        <section>
            <div class="flex items-center mb-10 justify-center">
                <div class="bg-blue-900 text-white px-8 py-3 rounded-full shadow-lg">
                    <h2 class="text-2xl font-bold">แผนการดำเนินงาน (30-45 วัน)</h2>
                </div>
            </div>

            <div class="relative wrap overflow-hidden p-4 md:p-10 h-full">
                <!-- Vertical Line -->
                <div class="border-2-2 absolute border-opacity-20 border-gray-700 h-full border" style="left: 50%"></div>

                <!-- Phase 1 -->
                <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-blue-900 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">1</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-l-4 border-blue-900">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">Planning & Setup</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 1</p>
                        <p class="text-gray-700 text-sm">จดโดเมนเนม, เตรียม Hosting, ติดตั้ง SSL และวางแผน Branding</p>
                    </div>
                </div>

                <!-- Phase 2 -->
                <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-cyan-600 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">2</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-r-4 border-cyan-600 text-right">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">System Installation</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 2</p>
                        <p class="text-gray-700 text-sm">ติดตั้ง WordPress, Theme และ Plugins ที่จำเป็น (Security, Backup, SEO)</p>
                    </div>
                </div>

                <!-- Phase 3 -->
                <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-blue-700 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">3</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-l-4 border-blue-700">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">Design & Dev</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 2-3</p>
                        <p class="text-gray-700 text-sm">ออกแบบ UX/UI, สร้างหน้า Home, Profile, Policy และ Contact ตาม Mood & Tone</p>
                    </div>
                </div>

                <!-- Phase 4 -->
                <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-cyan-500 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">4</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-r-4 border-cyan-500 text-right">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">Content Setup</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 3-4</p>
                        <p class="text-gray-700 text-sm">ลงเนื้อหา, รูปภาพ, เชื่อมต่อ Social Media และใส่ข้อความทางกฎหมาย (Disclaimer)</p>
                    </div>
                </div>

                 <!-- Phase 5 -->
                 <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-amber-500 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">5</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-l-4 border-amber-500">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">Testing & Review</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 4-5</p>
                        <p class="text-gray-700 text-sm">ทดสอบระบบความปลอดภัย, ความเร็ว, การแสดงผลมือถือ และแก้ไขงาน</p>
                    </div>
                </div>

                 <!-- Phase 6 -->
                 <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-emerald-500 shadow-xl w-12 h-12 rounded-full justify-center text-white font-bold">6</div>
                    <div class="order-1 w-5/12 px-6 py-4 bg-white rounded-lg shadow-xl hover:shadow-2xl transition-all border-r-4 border-emerald-500 text-right">
                        <h3 class="mb-3 font-bold text-gray-800 text-xl">Delivery (Go Live)</h3>
                        <p class="text-sm text-gray-600 mb-2">สัปดาห์ที่ 5-6</p>
                        <p class="text-gray-700 text-sm">เปิดใช้งานจริง, ส่งมอบคู่มือ และอบรมการใช้งานเบื้องต้น</p>
                    </div>
                </div>

            </div>
        </section>

        <!-- Section 5: Budget (Chart.js Doughnut - Goal: Compare/Composition) -->
        <section class="bg-gradient-to-br from-gray-900 to-blue-900 rounded-3xl p-8 md:p-12 text-white shadow-2xl">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                
                <div>
                    <h2 class="text-3xl font-bold mb-6 text-cyan-400">โครงสร้างงบประมาณ (Investment)</h2>
                    <p class="mb-6 text-gray-300">
                        การลงทุนในโครงการนี้เน้นที่การพัฒนาและออกแบบเป็นหลัก เพื่อให้ได้ระบบที่มั่นคงและสวยงาม โดยมีค่าใช้จ่ายส่วนอื่นๆ เป็นส่วนเสริม
                    </p>
                    <div class="space-y-4">
                        <div class="flex items-center p-3 bg-white/10 rounded-lg backdrop-blur-sm">
                            <div class="w-4 h-4 rounded-full bg-cyan-400 mr-3"></div>
                            <span class="font-semibold">ค่าบริการออกแบบและพัฒนา (Design & Dev)</span>
                            <span class="ml-auto text-cyan-300 font-mono">Core Cost</span>
                        </div>
                        <div class="flex items-center p-3 bg-white/10 rounded-lg backdrop-blur-sm">
                            <div class="w-4 h-4 rounded-full bg-amber-500 mr-3"></div>
                            <span class="font-semibold">โดเมนและโฮสติ้ง (Domain & Hosting)</span>
                            <span class="ml-auto text-amber-300 font-mono">Actual Cost</span>
                        </div>
                        <div class="flex items-center p-3 bg-white/10 rounded-lg backdrop-blur-sm">
                            <div class="w-4 h-4 rounded-full bg-blue-500 mr-3"></div>
                            <span class="font-semibold">ดูแลหลังการขาย (Maintenance)</span>
                            <span class="ml-auto text-blue-300 font-mono">Optional</span>
                        </div>
                    </div>
                </div>

                <div class="flex flex-col items-center">
                    <div class="chart-container">
                        <canvas id="budgetChart"></canvas>
                    </div>
                    <p class="mt-4 text-sm text-gray-400 italic">*ตัวเลขงบประมาณเป็นการประมาณการสัดส่วน</p>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="text-center py-12 border-t border-gray-200">
            <h3 class="text-2xl font-bold text-blue-900 mb-4">พร้อมยกระดับการสื่อสารสู่ยุคดิจิทัล</h3>
            <p class="text-gray-600 mb-8 max-w-2xl mx-auto">
                เว็บไซต์ที่ดีไม่ใช่แค่หน้าเพจ แต่คือเครื่องมือสร้างความเชื่อมั่นให้กับประชาชน
            </p>
            <button class="bg-gradient-to-r from-blue-700 to-cyan-600 text-white font-bold py-3 px-8 rounded-full shadow-lg hover:scale-105 transform transition duration-300">
                อนุมัติโครงการ
            </button>
            <p class="mt-8 text-xs text-gray-400">เอกสารข้อเสนอโครงการเว็บไซต์ผู้สมัคร สส.</p>
        </footer>

    </main>

    <script>
        // --- Helper Function: String Wrap for Labels ---
        function formatLabel(str, maxwidth) {
            var sections = [];
            var words = str.split(" ");
            var temp = "";
            words.forEach(function(item, index) {
                if (temp.length > 0) {
                    var concat = temp + ' ' + item;
                    if (concat.length > maxwidth) {
                        sections.push(temp);
                        temp = "";
                    } else {
                        if (index == (words.length - 1)) {
                            sections.push(concat);
                            return;
                        } else {
                            temp = concat;
                            return;
                        }
                    }
                }
                if (index == (words.length - 1)) {
                    sections.push(item);
                    return;
                }
                if (item.length < maxwidth) {
                    temp = item;
                } else {
                    sections.push(item);
                }
            });
            return sections;
        }

        // --- Chart 1: Tech Radar Chart ---
        const ctxRadar = document.getElementById('techRadarChart').getContext('2d');
        const radarData = {
            labels: [
                'ความปลอดภัย (Security)', 
                'ความเร็ว (Speed/Performance)', 
                'การรองรับมือถือ (Mobile Responsive)', 
                'ความสวยงาม (UX/UI Design)', 
                'เนื้อหา & กฎหมาย (Content & Legal)'
            ],
            datasets: [{
                label: 'ระดับความสำคัญ',
                data: [95, 90, 100, 85, 95], // High priority on Mobile, Security, Legal
                fill: true,
                backgroundColor: 'rgba(6, 182, 212, 0.2)', // Cyan transparent
                borderColor: '#06b6d4',
                pointBackgroundColor: '#1e3a8a',
                pointBorderColor: '#fff',
                pointHoverBackgroundColor: '#fff',
                pointHoverBorderColor: '#1e3a8a'
            }]
        };

        // Process labels for Radar
        const processedRadarLabels = radarData.labels.map(label => formatLabel(label, 16));

        new Chart(ctxRadar, {
            type: 'radar',
            data: {
                labels: processedRadarLabels,
                datasets: radarData.datasets
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    r: {
                        angleLines: { color: 'rgba(0, 0, 0, 0.1)' },
                        grid: { color: 'rgba(0, 0, 0, 0.1)' },
                        pointLabels: {
                            font: { size: 11, family: 'Sarabun' },
                            color: '#4b5563' // Gray-600
                        },
                        suggestedMin: 50,
                        suggestedMax: 100
                    }
                },
                plugins: {
                    legend: { display: false },
                    tooltip: {
                        callbacks: {
                            title: function(tooltipItems) {
                                const item = tooltipItems[0];
                                let label = item.chart.data.labels[item.dataIndex];
                                if (Array.isArray(label)) return label.join(' ');
                                return label;
                            }
                        }
                    }
                }
            }
        });

        // --- Chart 2: Budget Doughnut Chart ---
        const ctxDoughnut = document.getElementById('budgetChart').getContext('2d');
        const budgetData = {
            labels: [
                'ค่าบริการออกแบบและพัฒนา (Design & Dev)', 
                'โดเมนและโฮสติ้ง (Domain & Hosting)', 
                'บริการดูแลหลังการขาย (Maintenance)'
            ],
            datasets: [{
                data: [70, 20, 10], // Estimated split
                backgroundColor: [
                    '#22d3ee', // Cyan-400
                    '#f59e0b', // Amber-500
                    '#3b82f6'  // Blue-500
                ],
                hoverOffset: 4,
                borderWidth: 0
            }]
        };

        // Process labels for Doughnut
        const processedBudgetLabels = budgetData.labels.map(label => formatLabel(label, 20));

        new Chart(ctxDoughnut, {
            type: 'doughnut',
            data: {
                labels: processedBudgetLabels,
                datasets: budgetData.datasets
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                cutout: '65%',
                plugins: {
                    legend: {
                        display: false // Custom legend used in HTML
                    },
                    tooltip: {
                        backgroundColor: 'rgba(0,0,0,0.8)',
                        callbacks: {
                            title: function(tooltipItems) {
                                const item = tooltipItems[0];
                                let label = item.chart.data.labels[item.dataIndex];
                                if (Array.isArray(label)) return label.join(' ');
                                return label;
                            },
                            label: function(context) {
                                return ' ' + context.parsed + '% โดยประมาณ';
                            }
                        }
                    }
                }
            }
        });
    </script>
</body>
</html>
