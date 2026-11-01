# ECU-volleyball-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ECU Volleyball Team Hub</title>
    <style>
        :root {
            --primary: #0a192f;
            --secondary: #172a45;
            --accent: #f5a623;
            --text-light: #f8fafc;
            --text-muted: #94a3b8;
            --card-bg: #1e293b;
            --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: var(--font-main);
        }

        body {
            background-color: var(--primary);
            color: var(--text-light);
            line-height: 1.6;
        }

        header {
            background-color: var(--secondary);
            border-bottom: 3px solid var(--accent);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--accent);
            letter-spacing: 1px;
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 600;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--accent);
        }

        .hero {
            text-align: center;
            padding: 4rem 1rem;
            background: linear-gradient(180deg, var(--secondary) 0%, var(--primary) 100%);
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
            text-transform: uppercase;
        }

        .hero p {
            color: var(--text-muted);
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 2rem auto;
        }

        .cta-btn {
            background-color: var(--accent);
            color: var(--primary);
            padding: 0.8rem 1.8rem;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            display: inline-block;
            transition: transform 0.2s, background-color 0.2s;
        }

        .cta-btn:hover {
            transform: translateY(-2px);
            background-color: #e09216;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 3rem 1rem;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 2rem;
            color: var(--accent);
            text-transform: uppercase;
        }

        /* Grid Layouts */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background-color: var(--card-bg);
            border-radius: 8px;
            padding: 1.5rem;
            border-left: 4px solid var(--accent);
        }

        .card h3 {
            margin-bottom: 0.5rem;
            color: var(--text-light);
        }

        .card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* Match Schedule */
        .fixture {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: var(--card-bg);
            padding: 1rem 1.5rem;
            border-radius: 8px;
            margin-bottom: 1rem;
        }

        .fixture .teams {
            font-weight: bold;
            font-size: 1.1rem;
        }

        .fixture .details {
            color: var(--accent);
            font-size: 0.9rem;
            text-align: right;
        }

        /* Form Styling */
        form {
            background-color: var(--secondary);
            padding: 2rem;
            border-radius: 8px;
            max-width: 600px;
            margin: 0 auto;
            border: 1px solid #233554;
        }

        .form-group {
            margin-bottom: 1.2rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .form-group input, .form-group select {
            width: 100%;
            padding: 0.75rem;
            border-radius: 4px;
            border: 1px solid #233554;
            background-color: var(--primary);
            color: var(--text-light);
            font-size: 1rem;
        }

        .form-group input[type="file"] {
            padding: 0.4rem;
        }

        form button {
            width: 100%;
            padding: 0.8rem;
            background-color: var(--accent);
            color: var(--primary);
            border: none;
            border-radius: 4px;
            font-weight: bold;
            font-size: 1.1rem;
            cursor: pointer;
        }

        footer {
            text-align: center;
            padding: 2rem;
            background-color: var(--secondary);
            color: var(--text-muted);
            font-size: 0.9rem;
            border-top: 1px solid #233554;
            margin-top: 3rem;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">ECU VOLLEYBALL</div>
        <nav>
            <a href="#roster">Roster</a>
            <a href="#fixtures">Fixtures</a>
            <a href="#register">Register</a>
            <a href="#docs">Documents</a>
        </nav>
    </header>

    <section class="hero">
        <h1>ECU Volleyball Team Portal</h1>
        <p>Official hub for players, match fixtures, team announcements, and official player registration.</p>
        <a href="#register" class="cta-btn">Join The Squad</a>
    </section>

    <div class="container">
        <!-- Upcoming Fixtures -->
        <section id="fixtures" style="margin-bottom: 4rem;">
            <h2 class="section-title">Upcoming Fixtures</h2>
            <div class="fixture">
                <div class="teams">ECU Volleyball vs. Visiting Squad</div>
                <div class="details">Home Court | Match Date TBD</div>
            </div>
            <div class="fixture">
                <div class="teams">Internal Squad Scrimmage (A vs. B)</div>
                <div class="details">Main Court | Training Session</div>
            </div>
        </section>

        <!-- Squad Roster Overview -->
        <section id="roster" style="margin-bottom: 4rem;">
            <h2 class="section-title">Squad Focus & Structure</h2>
            <div class="grid">
                <div class="card">
                    <h3>Setters & Playmakers</h3>
                    <p>Focusing on court vision, quick rotation setups, and precise ball placement for attacks.</p>
                </div>
                <div class="card">
                    <h3>Outside & Opposite Hitters</h3>
                    <p>Dominant wing attacks, transition mechanics, and strong blocking setups.</p>
                </div>
                <div class="card">
                    <h3>Middle Blockers & Defense</h3>
                    <p>Fast net defense, lateral quickness, and strategic serve-receive positioning.</p>
                </div>
            </div>
        </section>

        <!-- Player Registration -->
        <section id="register" style="margin-bottom: 4rem;">
            <h2 class="section-title">Player Registration</h2>
            <form id="registrationForm">
                <div class="form-group">
                    <label for="fullname">Full Name</label>
                    <input type="text" id="fullname" required placeholder="Enter full name">
                </div>
                <div class="form-group">
                    <label for="level">Academic Level / Year</label>
                    <input type="text" id="level" placeholder="e.g., 100L, 200L, 400L" required>
                </div>
                <div class="form-group">
                    <label for="position">Preferred Position</label>
                    <select id="position" required>
                        <option value="">Select Position</option>
                        <option value="Setter">Setter</option>
                        <option value="Outside Hitter">Outside Hitter</option>
                        <option value="Opposite Hitter">Opposite Hitter</option>
                        <option value="Middle Blocker">Middle Blocker</option>
                        <option value="Libero">Libero</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="photo">Passport Photo Upload</label>
                    <input type="file" id="photo" accept="image/*" required>
                </div>
                <button type="submit">Submit Registration</button>
            </form>
        </section>

        <!-- Official Documents Section -->
        <section id="docs">
            <h2 class="section-title">Team Resources & Downloads</h2>
            <div class="grid">
                <div class="card" style="text-align: center;">
                    <h3>Code of Conduct</h3>
                    <p>Official rules regarding punctuality, practice discipline, and squad expectations.</p>
                    <br>
                    <a href="#" class="cta-btn" style="padding: 0.5rem 1rem; font-size: 0.9rem;">Download PDF</a>
                </div>
                <div class="card" style="text-align: center;">
                    <h3>Court Guidelines</h3>
                    <p>Training schedules, gear requirements, and team physical conditioning plans.</p>
                    <br>
                    <a href="#" class="cta-btn" style="padding: 0.5rem 1rem; font-size: 0.9rem;">Download PDF</a>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <p>&copy; ECU Volleyball Team | All Rights Reserved</p>
    </footer>

    <script>
        document.getElementById('registrationForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const name = document.getElementById('fullname').value;
            alert(`Thank you ${name}, your registration details have been submitted!`);
            this.reset();
        });
    </script>
</body>
</html>
