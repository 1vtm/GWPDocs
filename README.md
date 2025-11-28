<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Group Watch Pro - User Guide</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            overflow: hidden;
        }

        header {
            background: linear-gradient(135deg, #5865F2 0%, #5865F2 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }

        header p {
            font-size: 1.3em;
            opacity: 0.9;
        }

        .content {
            padding: 40px;
        }

        h2 {
            color: #5865F2;
            font-size: 2em;
            margin: 40px 0 20px 0;
            padding-bottom: 10px;
            border-bottom: 3px solid #5865F2;
        }

        h3 {
            color: #764ba2;
            font-size: 1.5em;
            margin: 30px 0 15px 0;
        }

        h4 {
            color: #667eea;
            font-size: 1.2em;
            margin: 20px 0 10px 0;
        }

        p {
            margin: 15px 0;
            font-size: 1.1em;
        }

        ul, ol {
            margin: 15px 0 15px 30px;
        }

        li {
            margin: 10px 0;
            font-size: 1.05em;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .feature-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #5865F2;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-5px);
        }

        .feature-card h3 {
            margin-top: 0;
            color: #5865F2;
        }

        .command-box {
            background: #2d2d2d;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 8px;
            font-family: 'Courier New', monospace;
            margin: 15px 0;
            border-left: 4px solid #5865F2;
            overflow-x: auto;
        }

        .command-box code {
            font-size: 1em;
        }

        .premium-section {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
        }

        .premium-section h2,
        .premium-section h3 {
            color: white;
            border-bottom: 2px solid rgba(255,255,255,0.3);
        }

        .tips-box {
            background: #fff3cd;
            border-left: 5px solid #ffc107;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }

        .help-box {
            background: #d1ecf1;
            border-left: 5px solid #17a2b8;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }

        .checklist {
            background: #d4edda;
            border-left: 5px solid #28a745;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }

        .checklist ul {
            list-style: none;
            margin-left: 0;
        }

        .checklist li:before {
            content: "☐ ";
            margin-right: 10px;
            font-size: 1.2em;
        }

        .highlight {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            text-align: center;
        }

        .highlight ul {
            list-style: none;
            margin: 20px 0;
        }

        .highlight li {
            margin: 10px 0;
            font-size: 1.1em;
        }

        .highlight li:before {
            content: "✅ ";
            margin-right: 10px;
        }

        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }

        .category-item {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 10px;
            border: 2px solid #e9ecef;
            transition: all 0.3s;
        }

        .category-item:hover {
            border-color: #5865F2;
            transform: scale(1.02);
        }

        .faq-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin: 15px 0;
            border-left: 4px solid #5865F2;
        }

        .faq-item strong {
            color: #5865F2;
            display: block;
            margin-bottom: 10px;
            font-size: 1.1em;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        table th,
        table td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        table th {
            background: #5865F2;
            color: white;
        }

        table tr:hover {
            background: #f5f5f5;
        }

        .quick-ref {
            background: linear-gradient(135deg, #84fab0 0%, #8fd3f4 100%);
            padding: 25px;
            border-radius: 15px;
            margin: 30px 0;
        }

        .quick-ref h3 {
            color: #2d3748;
            margin-top: 0;
        }

        .quick-ref ul {
            columns: 2;
            column-gap: 30px;
        }

        footer {
            background: #2d2d2d;
            color: white;
            text-align: center;
            padding: 30px;
            margin-top: 40px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2em;
            }

            .content {
                padding: 20px;
            }

            .feature-grid {
                grid-template-columns: 1fr;
            }

            .quick-ref ul {
                columns: 1;
            }
        }

        .emoji {
            font-size: 1.2em;
        }

        a {
            color: #5865F2;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🎬 Group Watch Pro</h1>
            <p>Your Ultimate Discord Community Bot</p>
        </header>

        <div class="content">
            <section>
                <h2>👋 Welcome to Group Watch Pro!</h2>
                <p>Group Watch Pro is a powerful, feature-rich Discord bot designed to enhance your server experience. Whether you're looking to manage your community, entertain members, or create engaging experiences, Group Watch Pro has everything you need.</p>
            </section>

            <section>
                <h2>🌟 What is Group Watch Pro?</h2>
                <p>Group Watch Pro is an all-in-one Discord bot that brings professional community management tools, entertainment features, and premium capabilities to your server. With over <strong>90 commands</strong> and countless features, it's the perfect companion for any Discord community.</p>
            </section>

            <section>
                <h2>✨ Key Features</h2>
                <div class="feature-grid">
                    <div class="feature-card">
                        <h3>🎵 Advanced Music System</h3>
                        <ul>
                            <li>Play music from YouTube, SoundCloud, and more</li>
                            <li>Queue management with easy controls</li>
                            <li>Create and save playlists</li>
                            <li>Volume control and loop modes</li>
                            <li>Shuffle your queue</li>
                            <li>View song lyrics instantly</li>
                        </ul>
                    </div>

                    <div class="feature-card">
                        <h3>🛡️ Powerful Moderation</h3>
                        <ul>
                            <li>Automatic moderation with spam detection</li>
                            <li>Warning system with automatic actions</li>
                            <li>Kick, ban, and timeout users</li>
                            <li>Message purging</li>
                            <li>Banned word filtering</li>
                            <li>Link protection</li>
                        </ul>
                    </div>

                    <div class="feature-card">
                        <h3>🎉 Engagement Features</h3>
                        <ul>
                            <li>Automated giveaways with multiple winners</li>
                            <li>Create polls with reactions</li>
                            <li>Leveling system with XP and rewards</li>
                            <li>Virtual economy with daily rewards</li>
                            <li>Mini-games for entertainment</li>
                            <li>Birthday tracking and announcements</li>
                        </ul>
                    </div>

                    <div class="feature-card">
                        <h3>🎫 Support System</h3>
                        <ul>
                            <li>Easy-to-use ticket system</li>
                            <li>Button-based ticket creation</li>
                            <li>User management in tickets</li>
                            <li>Automatic channel organization</li>
                        </ul>
                    </div>

                    <div class="feature-card">
                        <h3>📢 Professional Announcements</h3>
                        <ul>
                            <li>Beautifully formatted announcements</li>
                            <li>Multiple style presets</li>
                            <li>Update posts with changelogs</li>
                            <li>Event announcements</li>
                            <li>Role pinging support</li>
                        </ul>
                    </div>

                    <div class="feature-card">
                        <h3>📊 Community Tools</h3>
                        <ul>
                            <li>Server statistics and analytics</li>
                            <li>Invite tracking and leaderboards</li>
                            <li>Suggestion system with voting</li>
                            <li>Starboard for popular messages</li>
                            <li>Welcome messages for new members</li>
                            <li>AFK status management</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section>
                <h2>🎮 Getting Started</h2>
                <h3>Basic Commands</h3>
                
                <p><strong>Need help?</strong></p>
                <div class="command-box">
                    <code>/help</code>
                </div>
                <p>View all available commands organized by category.</p>

                <p><strong>Check bot status:</strong></p>
                <div class="command-box">
                    <code>/ping</code>
                </div>
                <p>See the bot's response time and latency.</p>

                <p><strong>View server info:</strong></p>
                <div class="command-box">
                    <code>/utility</code>
                </div>
                <p>Access utility tools like server stats, user info, and more.</p>
            </section>

            <section>
                <h2>🎵 Music Commands</h2>
                <h3>Playing Music</h3>

                <p><strong>Play a song:</strong></p>
                <div class="command-box">
                    <code>/play query: [song name or URL]</code>
                </div>
                <p>Play music from YouTube, SoundCloud, or direct links. The bot will join your voice channel and start playing!</p>

                <p><strong>View the queue:</strong></p>
                <div class="command-box">
                    <code>/queue</code>
                </div>
                <p>See what's playing next and manage your queue.</p>

                <p><strong>Skip a song:</strong></p>
                <div class="command-box">
                    <code>/skip</code>
                </div>
                <p>Jump to the next song in the queue.</p>

                <p><strong>Control playback:</strong></p>
                <p>When music is playing, you'll see buttons for:</p>
                <ul>
                    <li>⏸️ Pause/Resume</li>
                    <li>⏭️ Skip</li>
                    <li>⏹️ Stop</li>
                    <li>🔊 Volume</li>
                    <li>🔁 Loop</li>
                </ul>

                <p><strong>Other music commands:</strong></p>
                <ul>
                    <li><code>/loop</code> - Set loop mode (song, queue, or off)</li>
                    <li><code>/shuffle</code> - Randomize your queue</li>
                    <li><code>/music-history</code> - View recently played songs</li>
                    <li><code>/lyrics</code> - Get lyrics for any song</li>
                    <li><code>/queue-remove</code> - Remove a song from queue</li>
                    <li><code>/queue-clear</code> - Clear the entire queue</li>
                </ul>

                <h3>Playlists</h3>
                <p><strong>Create a playlist:</strong></p>
                <div class="command-box">
                    <code>/playlists</code>
                </div>
                <p>Use the buttons to create, add songs, and manage your playlists.</p>

                <p><strong>Play a playlist:</strong></p>
                <div class="command-box">
                    <code>/playlists</code>
                </div>
                <p>Select "Play" to queue an entire playlist.</p>
            </section>

            <section>
                <h2>🛡️ Moderation (Admin Only)</h2>
                <h3>Warning System</h3>

                <p><strong>Warn a user:</strong></p>
                <div class="command-box">
                    <code>/warn user: @user reason: [reason]</code>
                </div>
                <p>Issue warnings that can trigger automatic actions.</p>

                <p><strong>View warnings:</strong></p>
                <div class="command-box">
                    <code>/warnings user: @user</code>
                </div>

                <p><strong>Clear warnings:</strong></p>
                <div class="command-box">
                    <code>/clear-warnings user: @user</code>
                </div>

                <h3>Moderation Actions</h3>
                <div class="command-box">
                    <code>/kick user: @user reason: [reason]</code>
                </div>
                <div class="command-box">
                    <code>/ban user: @user reason: [reason] delete_days: [0-7]</code>
                </div>
                <div class="command-box">
                    <code>/timeout user: @user duration: 1h reason: [reason]</code>
                </div>
                <div class="command-box">
                    <code>/untimeout user: @user</code>
                </div>
                <div class="command-box">
                    <code>/purge amount: 50 user: @user (optional)</code>
                </div>
            </section>

            <section>
                <h2>🎉 Giveaways</h2>
                <h3>Creating Giveaways</h3>

                <p><strong>Start a giveaway:</strong></p>
                <div class="command-box">
                    <code>/giveaways action: start duration: 60 winners: 1 prize: Discord Nitro</code>
                </div>
                <ul>
                    <li><strong>Duration:</strong> How long the giveaway lasts (in minutes)</li>
                    <li><strong>Winners:</strong> Number of winners to select</li>
                    <li><strong>Prize:</strong> What you're giving away</li>
                </ul>

                <p><strong>End a giveaway early:</strong></p>
                <div class="command-box">
                    <code>/giveaways action: end message_id: [message ID]</code>
                </div>

                <p><strong>Reroll winners:</strong></p>
                <div class="command-box">
                    <code>/giveaways action: reroll message_id: [message ID]</code>
                </div>

                <h3>How Giveaways Work</h3>
                <ol>
                    <li>Admin creates a giveaway with <code>/giveaways</code></li>
                    <li>Members react with 🎉 to enter</li>
                    <li>Bot automatically ends the giveaway at the specified time</li>
                    <li>Winners are randomly selected and announced</li>
                    <li>Admins can reroll if needed</li>
                </ol>
            </section>

            <section>
                <h2>🎫 Tickets</h2>
                <h3>Creating Tickets</h3>

                <p><strong>For Admins - Create ticket panel:</strong></p>
                <div class="command-box">
                    <code>/tickets action: panel</code>
                </div>
                <p>This creates a button that members can click to create tickets.</p>

                <p><strong>For Members - Create a ticket:</strong></p>
                <ol>
                    <li>Click the "📩 Create Ticket" button in the ticket panel</li>
                    <li>A private channel is created just for you</li>
                    <li>Staff members can join to help you</li>
                </ol>

                <p><strong>For Admins - Manage tickets:</strong></p>
                <div class="command-box">
                    <code>/tickets action: manage</code>
                </div>
                <p>Use this in a ticket channel to add/remove users or close the ticket.</p>

                <p><strong>Close a ticket:</strong></p>
                <div class="command-box">
                    <code>/ticket-close</code>
                </div>
                <p>Closes the current ticket channel (5 second countdown).</p>
            </section>

            <section>
                <h2>📢 Announcements</h2>
                <h3>Making Announcements</h3>

                <p><strong>Basic announcement:</strong></p>
                <div class="command-box">
                    <code>/announce channel: #announcements title: Server Update message: We have new features! style: celebration</code>
                </div>

                <p><strong>Announcement styles:</strong></p>
                <ul>
                    <li><code>default</code> - Standard blue</li>
                    <li><code>important</code> - Red (urgent)</li>
                    <li><code>celebration</code> - Gold (events)</li>
                    <li><code>warning</code> - Orange (caution)</li>
                    <li><code>info</code> - Light blue (information)</li>
                </ul>

                <p><strong>Post an update:</strong></p>
                <div class="command-box">
                    <code>/updates channel: #updates version: v2.0.0 title: Major Update changes: New features | Bug fixes | Improvements</code>
                </div>
                <p>Use <code>|</code> to separate bullet points.</p>

                <p><strong>Create an event:</strong></p>
                <div class="command-box">
                    <code>/event-announce channel: #events event_name: Movie Night description: Join us for a movie! date_time: Friday 8 PM EST location: #voice-channel</code>
                </div>
            </section>

            <section>
                <h2>🎮 Games & Entertainment</h2>
                <h3>Mini-Games</h3>

                <p><strong>Play games:</strong></p>
                <div class="command-box">
                    <code>/games</code>
                </div>
                <p>Access mini-games via buttons:</p>
                <ul>
                    <li>🎱 <strong>8ball</strong> - Ask the magic 8-ball a question</li>
                    <li>🪙 <strong>Coinflip</strong> - Flip a coin</li>
                    <li>🎲 <strong>Dice</strong> - Roll dice</li>
                    <li>✂️ <strong>RPS</strong> - Rock Paper Scissors</li>
                    <li>🧠 <strong>Trivia</strong> - Answer trivia questions</li>
                </ul>
            </section>

            <section>
                <h2>💰 Economy System</h2>
                <h3>Earning Coins</h3>

                <p><strong>Claim daily reward:</strong></p>
                <div class="command-box">
                    <code>/economy</code>
                </div>
                <p>Click the "Daily" button to claim your daily coins!</p>

                <p><strong>Work for coins:</strong></p>
                <div class="command-box">
                    <code>/economy</code>
                </div>
                <p>Click the "Work" button to earn coins by working.</p>

                <h3>Spending Coins</h3>
                <p><strong>View shop:</strong></p>
                <div class="command-box">
                    <code>/economy</code>
                </div>
                <p>Click the "Shop" button to see available items.</p>

                <p><strong>Pay another user:</strong></p>
                <div class="command-box">
                    <code>/pay user: @user amount: 100</code>
                </div>
            </section>

            <section>
                <h2>📈 Leveling System</h2>
                <h3>Earning XP</h3>
                <ul>
                    <li>Send messages in the server</li>
                    <li>XP is awarded randomly (10-25 XP per message)</li>
                    <li>60 second cooldown between XP gains</li>
                    <li>Level up by earning enough XP</li>
                </ul>

                <h3>Leveling Commands</h3>
                <div class="command-box">
                    <code>/rank</code>
                </div>
                <p>See your level, XP, and progress to next level.</p>

                <div class="command-box">
                    <code>/leaderboard</code>
                </div>
                <p>See the top members by XP.</p>
            </section>

            <section>
                <h2>📊 Utility Commands</h2>
                <p><strong>Access utilities:</strong></p>
                <div class="command-box">
                    <code>/utility</code>
                </div>
                <p>Use buttons to access:</p>
                <ul>
                    <li>🖼️ <strong>Avatar</strong> - View user avatars</li>
                    <li>👤 <strong>User Info</strong> - Detailed user information</li>
                    <li>📊 <strong>Server Stats</strong> - Server statistics</li>
                    <li>📺 <strong>Channel Info</strong> - Channel details</li>
                    <li>🖼️ <strong>Banner</strong> - Server banner</li>
                    <li>🎭 <strong>Role Info</strong> - Role information</li>
                </ul>
            </section>

            <section>
                <h2>😴 Social Features</h2>
                <h3>AFK System</h3>
                <div class="command-box">
                    <code>/afk reason: Away for lunch</code>
                </div>
                <p>When someone mentions you, they'll see your AFK status.</p>

                <h3>Birthday System</h3>
                <div class="command-box">
                    <code>/birthday-set date: 12/25</code>
                </div>
                <p>Format: MM/DD (month/day)</p>
            </section>

            <section>
                <h2>💭 Community Features</h2>
                <h3>Suggestions</h3>
                <div class="command-box">
                    <code>/suggest suggestion: Add a music channel</code>
                </div>
                <p>Your suggestion will be posted in the suggestions channel with voting reactions.</p>

                <h3>Starboard</h3>
                <p>When a message gets enough ⭐ reactions, it's automatically posted to the starboard channel!</p>
            </section>

            <section>
                <h2>🔗 Invite Tracking</h2>
                <div class="command-box">
                    <code>/invites</code>
                </div>
                <p>See your invite statistics including total invites, valid invites, and more.</p>

                <div class="command-box">
                    <code>/invite-leaderboard</code>
                </div>
                <p>See who's invited the most members.</p>
            </section>

            <section>
                <h2>⏰ Reminders</h2>
                <div class="command-box">
                    <code>/remind time: 2h message: Check server updates</code>
                </div>
                <p>Time formats: <code>30m</code>, <code>1h</code>, <code>2d</code>, etc.</p>

                <div class="command-box">
                    <code>/reminders</code>
                </div>
                <p>See all your active reminders.</p>
            </section>

            <section>
                <h2>📝 Polls</h2>
                <div class="command-box">
                    <code>/poll-create question: Best feature? options: Music | Moderation | Giveaways duration: 60</code>
                </div>
                <ul>
                    <li>Separate options with <code>|</code></li>
                    <li>Max 10 options</li>
                    <li>Duration in minutes (optional)</li>
                </ul>
            </section>

            <section class="premium-section">
                <h2>⭐ Premium Features</h2>
                <h3>What is Premium?</h3>
                <p>Premium unlocks advanced features and exclusive commands to enhance your server experience even further.</p>

                <h3>Premium Tiers</h3>
                <ul>
                    <li><strong>Daily</strong> - 24 hours of premium access</li>
                    <li><strong>Weekly</strong> - 7 days of premium access</li>
                    <li><strong>Monthly</strong> - 30 days of premium access</li>
                    <li><strong>Lifetime</strong> - Permanent premium access</li>
                </ul>

                <h3>Premium Perks</h3>
                <div class="command-box">
                    <code>/premium-perks</code>
                </div>
                <p>View all premium features.</p>

                <h4>🌟 Advanced Announcements</h4>
                <p>Create stunning announcements with:</p>
                <ul>
                    <li>Multiple embed support</li>
                    <li>Custom formatting options</li>
                    <li>Scheduled posting</li>
                    <li>Advanced styling</li>
                </ul>
                <div class="command-box">
                    <code>/premium-announce</code>
                </div>

                <h4>📊 Advanced Statistics</h4>
                <p>Get detailed insights about your server:</p>
                <ul>
                    <li>Member growth charts</li>
                    <li>Activity analytics</li>
                    <li>Command usage statistics</li>
                    <li>Engagement metrics</li>
                </ul>
                <div class="command-box">
                    <code>/advanced-stats</code>
                </div>

                <h4>🎨 Custom Embed Creator</h4>
                <p>Create fully customized embeds with:</p>
                <ul>
                    <li>Complete control over colors, images, and text</li>
                    <li>Multiple fields</li>
                    <li>Custom footers and authors</li>
                    <li>Professional formatting</li>
                </ul>
                <div class="command-box">
                    <code>/custom-embed</code>
                </div>

                <h4>🚀 Priority Support</h4>
                <ul>
                    <li>Faster response times</li>
                    <li>Priority bug fixes</li>
                    <li>Feature requests prioritized</li>
                    <li>Direct support access</li>
                </ul>

                <h3>Checking Premium Status</h3>
                <div class="command-box">
                    <code>/premium-status</code>
                </div>
                <p>Check your premium status.</p>

                <h3>Getting Premium</h3>
                <p>Contact your server administrator or bot owner to get premium access. Premium can be granted for individual users or entire servers.</p>
            </section>

            <section>
                <h2>🎯 Tips & Tricks</h2>
                <div class="tips-box">
                    <h3>Getting the Most Out of Group Watch Pro</h3>
                    <ol>
                        <li><strong>Use <code>/help</code></strong> - Explore all available commands</li>
                        <li><strong>Try button-based commands</strong> - Many commands have interactive buttons for easier use</li>
                        <li><strong>Check <code>/settings</code></strong> - Admins can configure everything to your server's needs</li>
                        <li><strong>Use <code>/dashboard</code></strong> - Admins get a quick overview of server settings</li>
                        <li><strong>Explore premium</strong> - Unlock advanced features with premium</li>
                    </ol>
                </div>

                <h3>Best Practices</h3>
                <p><strong>For Music:</strong></p>
                <ul>
                    <li>Use playlists for your favorite songs</li>
                    <li>Set loop mode for background music</li>
                    <li>Use shuffle for variety</li>
                </ul>

                <p><strong>For Moderation:</strong></p>
                <ul>
                    <li>Set up auto-moderation to prevent spam</li>
                    <li>Use warnings before bans</li>
                    <li>Configure logging to track actions</li>
                </ul>

                <p><strong>For Community:</strong></p>
                <ul>
                    <li>Create regular giveaways to boost engagement</li>
                    <li>Use polls for community decisions</li>
                    <li>Set up welcome messages for new members</li>
                </ul>
            </section>

            <section>
                <h2>🆘 Need Help?</h2>
                <div class="help-box">
                    <h3>Getting Support</h3>
                    <ol>
                        <li><strong>Use <code>/help</code></strong> - View all commands and descriptions</li>
                        <li><strong>Check command descriptions</strong> - Hover over commands in Discord to see details</li>
                        <li><strong>Contact server admins</strong> - They can help with server-specific issues</li>
                        <li><strong>Use tickets</strong> - Create a ticket for support if available</li>
                    </ol>
                </div>

                <h3>Common Questions</h3>
                <div class="faq-item">
                    <strong>Q: Why isn't the bot responding?</strong>
                    <p>A: Check if the bot is online (green status). If it's online, make sure you're using slash commands (/) and the bot has proper permissions.</p>
                </div>

                <div class="faq-item">
                    <strong>Q: How do I use music commands?</strong>
                    <p>A: Make sure you're in a voice channel first, then use <code>/play</code> with a song name or URL.</p>
                </div>

                <div class="faq-item">
                    <strong>Q: Can I use this bot in multiple servers?</strong>
                    <p>A: Yes! The bot works in any server it's invited to.</p>
                </div>

                <div class="faq-item">
                    <strong>Q: How do I get premium?</strong>
                    <p>A: Contact your server administrator or the bot owner.</p>
                </div>

                <div class="faq-item">
                    <strong>Q: Are there any command limits?</strong>
                    <p>A: No limits for users! Use commands as much as you want.</p>
                </div>
            </section>

            <section>
                <h2>🎉 Feature Highlights</h2>
                <div class="highlight">
                    <h3>What Makes Group Watch Pro Special?</h3>
                    <ul>
                        <li><strong>90+ Commands</strong> - Comprehensive feature set</li>
                        <li><strong>Button-Based UI</strong> - Modern, interactive interface</li>
                        <li><strong>Music System</strong> - Multi-platform music support</li>
                        <li><strong>Moderation Tools</strong> - Professional moderation suite</li>
                        <li><strong>Engagement Features</strong> - Keep your community active</li>
                        <li><strong>Premium Features</strong> - Advanced capabilities for power users</li>
                        <li><strong>Easy to Use</strong> - Intuitive commands and interfaces</li>
                        <li><strong>Highly Configurable</strong> - Customize everything to your needs</li>
                        <li><strong>Regular Updates</strong> - Constantly improving and adding features</li>
                        <li><strong>Active Support</strong> - Help when you need it</li>
                    </ul>
                </div>
            </section>

            <section>
                <h2>📚 Command Categories</h2>
                <div class="category-grid">
                    <div class="category-item">
                        <h4>🎵 Music</h4>
                        <p>Play, queue, skip, stop, loop, shuffle, lyrics, playlists</p>
                    </div>
                    <div class="category-item">
                        <h4>🛡️ Moderation</h4>
                        <p>Warn, kick, ban, timeout, purge, warnings</p>
                    </div>
                    <div class="category-item">
                        <h4>🎉 Giveaways</h4>
                        <p>Start, end, reroll giveaways</p>
                    </div>
                    <div class="category-item">
                        <h4>🎫 Tickets</h4>
                        <p>Create and manage support tickets</p>
                    </div>
                    <div class="category-item">
                        <h4>📢 Announcements</h4>
                        <p>Create formatted announcements, updates, events</p>
                    </div>
                    <div class="category-item">
                        <h4>🎮 Games</h4>
                        <p>8ball, coinflip, dice, rock paper scissors, trivia</p>
                    </div>
                    <div class="category-item">
                        <h4>💰 Economy</h4>
                        <p>Daily rewards, work, shop, pay, balance</p>
                    </div>
                    <div class="category-item">
                        <h4>📈 Leveling</h4>
                        <p>Rank, leaderboard, XP system</p>
                    </div>
                    <div class="category-item">
                        <h4>📊 Utility</h4>
                        <p>Avatar, user info, server stats, channel info</p>
                    </div>
                    <div class="category-item">
                        <h4>😴 Social</h4>
                        <p>AFK, birthdays</p>
                    </div>
                    <div class="category-item">
                        <h4>💭 Community</h4>
                        <p>Suggestions, starboard</p>
                    </div>
                    <div class="category-item">
                        <h4>⭐ Premium</h4>
                        <p>Advanced features and exclusive commands</p>
                    </div>
                </div>
            </section>

            <section>
                <h2>🚀 Getting Started Checklist</h2>
                <div class="checklist">
                    <h3>For New Users:</h3>
                    <ul>
                        <li>Use <code>/help</code> to explore commands</li>
                        <li>Try <code>/ping</code> to check bot status</li>
                        <li>Check <code>/rank</code> to see your level</li>
                        <li>Try <code>/games</code> for some fun</li>
                        <li>Set your birthday with <code>/birthday-set</code></li>
                        <li>Explore <code>/utility</code> for server info</li>
                    </ul>
                </div>

                <div class="checklist">
                    <h3>For Server Admins:</h3>
                    <ul>
                        <li>Configure <code>/settings</code> for your server</li>
                        <li>Set up <code>/welcomer</code> for new members</li>
                        <li>Configure <code>/automod</code> for protection</li>
                        <li>Create <code>/tickets</code> panel for support</li>
                        <li>Set up <code>/logging</code> for event tracking</li>
                        <li>Check <code>/dashboard</code> for overview</li>
                    </ul>
                </div>
            </section>

            <section>
                <h2>💡 Pro Tips</h2>
                <ol>
                    <li><strong>Use slash commands</strong> - Type <code>/</code> to see all available commands</li>
                    <li><strong>Read command descriptions</strong> - Hover over commands for details</li>
                    <li><strong>Try button interfaces</strong> - Many commands have interactive buttons</li>
                    <li><strong>Check <code>/help</code> regularly</strong> - New features are added frequently</li>
                    <li><strong>Explore premium</strong> - Advanced features await with premium</li>
                    <li><strong>Join the community</strong> - Connect with other users</li>
                    <li><strong>Give feedback</strong> - Help improve the bot with suggestions</li>
                </ol>
            </section>

            <section>
                <h2>🎊 Conclusion</h2>
                <p>Group Watch Pro is your all-in-one solution for Discord community management and entertainment. With powerful features, an intuitive interface, and premium capabilities, it's the perfect bot for any server.</p>
                <p><strong>Start exploring today with <code>/help</code>!</strong></p>
            </section>

            <section>
                <h2>📞 Quick Reference</h2>
                <div class="quick-ref">
                    <h3>Essential Commands:</h3>
                    <ul>
                        <li><code>/help</code> - View all commands</li>
                        <li><code>/ping</code> - Check bot status</li>
                        <li><code>/play</code> - Play music</li>
                        <li><code>/rank</code> - Check your level</li>
                        <li><code>/economy</code> - Access economy features</li>
                        <li><code>/utility</code> - View server info</li>
                        <li><code>/premium-perks</code> - See premium features</li>
                    </ul>

                    <h3>For Admins:</h3>
                    <ul>
                        <li><code>/settings</code> - Configure everything</li>
                        <li><code>/dashboard</code> - Server overview</li>
                        <li><code>/automod</code> - Set up moderation</li>
                        <li><code>/welcomer</code> - Welcome messages</li>
                        <li><code>/tickets</code> - Ticket system</li>
                    </ul>
                </div>
            </section>
        </div>

        <footer>
            <h3>Group Watch Pro v2.0</h3>
            <p>Your Ultimate Discord Community Bot</p>
            <p style="margin-top: 20px; opacity: 0.8;">Thank you for using Group Watch Pro! 🎉</p>
        </footer>
    </div>
</body>
</html>

