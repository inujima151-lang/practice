# practice
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>社内AI勉強会 Vol.1 - Future of Work</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['"Inter"', '"Noto Sans JP"', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#f0fdfa',
                            100: '#ccfbf1',
                            500: '#14b8a6',
                            600: '#0d9488',
                            900: '#111827', // Dark background
                            800: '#1f2937', // Card background
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #0f172a; /* Slate 900 */
            color: #e2e8f0; /* Slate 200 */
        }
        .gradient-text {
            background: linear-gradient(to right, #818cf8, #2dd4bf);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .glass-card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body class="antialiased leading-relaxed">

    <header class="relative pt-20 pb-32 overflow-hidden">
        <div class="absolute top-0 left-1/2 w-96 h-96 bg-indigo-600 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob -translate-x-1/2"></div>
        <div class="absolute top-0 right-1/2 w-96 h-96 bg-teal-600 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob translate-x-1/2 animation-delay-2000"></div>

        <div class="container mx-auto px-6 relative z-10 text-center">
            <span class="inline-block py-1 px-3 rounded-full bg-indigo-900/50 border border-indigo-500/30 text-indigo-300 text-sm font-medium mb-6">
                Internal Event / 社内限定
            </span>
            <h1 class="text-5xl md:text-7xl font-bold mb-6 tracking-tight">
                AI勉強会 <span class="gradient-text">Vol.1</span>
            </h1>
            <p class="text-xl text-slate-400 max-w-2xl mx-auto mb-10">
                生成AIが変える私たちの業務プロセス。<br>
                基礎知識から実際の活用事例まで、共に学び、議論しましょう。
            </p>
            <div class="flex justify-center gap-4 flex-col sm:flex-row">
                <a href="#register" class="px-8 py-4 bg-gradient-to-r from-indigo-600 to-teal-500 rounded-lg text-white font-bold shadow-lg hover:shadow-indigo-500/30 transition transform hover:-translate-y-1">
                    参加登録する
                </a>
                <a href="#agenda" class="px-8 py-4 bg-slate-800 border border-slate-700 rounded-lg text-slate-300 font-medium hover:bg-slate-700 transition">
                    アジェンダを見る
                </a>
            </div>
        </div>
    </header>

    <section class="container mx-auto px-6 -mt-20 relative z-20">
        <div class="grid md:grid-cols-3 gap-6">
            <div class="glass-card p-6 rounded-xl shadow-xl text-center">
                <div class="text-teal-400 mb-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                    </svg>
                </div>
                <h3 class="text-lg font-bold text-white">日時</h3>
                <p class="text-slate-400 mt-1">2024年XX月XX日(金)<br>18:00 - 20:00</p>
            </div>
            <div class="glass-card p-6 rounded-xl shadow-xl text-center">
                <div class="text-indigo-400 mb-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                    </svg>
                </div>
                <h3 class="text-lg font-bold text-white">場所</h3>
                <p class="text-slate-400 mt-1">本社 5F 会議室A<br>+ Zoom配信</p>
            </div>
            <div class="glass-card p-6 rounded-xl shadow-xl text-center">
                <div class="text-purple-400 mb-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z" />
                    </svg>
                </div>
                <h3 class="text-lg font-bold text-white">対象</h3>
                <p class="text-slate-400 mt-1">全社員対象<br>（エンジニア以外も歓迎）</p>
            </div>
        </div>
    </section>

    <section id="agenda" class="py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Agenda</h2>
                <p class="text-slate-400">当日のタイムスケジュール</p>
            </div>

            <div class="max-w-3xl mx-auto space-y-8">
                <div class="flex flex-col md:flex-row gap-6 items-start">
                    <div class="w-full md:w-32 text-right md:pt-1">
                        <span class="text-teal-400 font-mono text-xl font-bold">18:00</span>
                    </div>
                    <div class="flex-1 pb-8 border-l border-slate-700 pl-8 relative">
                        <div class="absolute -left-1.5 top-2 w-3 h-3 rounded-full bg-teal-500"></div>
                        <h3 class="text-xl font-bold text-white mb-2">オープニング & 背景共有</h3>
                        <p class="text-slate-400 text-sm">CTOより、なぜ今社内でAI活用を進めるのか、その戦略とビジョンについてお話しします。</p>
                    </div>
                </div>
                <div class="flex flex-col md:flex-row gap-6 items-start">
                    <div class="w-full md:w-32 text-right md:pt-1">
                        <span class="text-teal-400 font-mono text-xl font-bold">18:15</span>
                    </div>
                    <div class="flex-1 pb-8 border-l border-slate-700 pl-8 relative">
                        <div class="absolute -left-1.5 top-2 w-3 h-3 rounded-full bg-teal-500"></div>
                        <h3 class="text-xl font-bold text-white mb-2">【講演】生成AI基礎講座</h3>
                        <p class="text-slate-400 text-sm">LLMの仕組みから、プロンプトエンジニアリングの基本まで。開発部 佐藤氏によるわかりやすい解説。</p>
                    </div>
                </div>
                <div class="flex flex-col md:flex-row gap-6 items-start">
                    <div class="w-full md:w-32 text-right md:pt-1">
                        <span class="text-teal-400 font-mono text-xl font-bold">19:00</span>
                    </div>
                    <div class="flex-1 pb-8 border-l border-slate-700 pl-8 relative">
                        <div class="absolute -left-1.5 top-2 w-3 h-3 rounded-full bg-teal-500"></div>
                        <h3 class="text-xl font-bold text-white mb-2">【ワーク】業務改善アイデアソン</h3>
                        <p class="text-slate-400 text-sm">チームに分かれて、「自分の業務のどこにAIが使えるか」をディスカッションします。</p>
                    </div>
                </div>
                <div class="flex flex-col md:flex-row gap-6 items-start">
                    <div class="w-full md:w-32 text-right md:pt-1">
                        <span class="text-teal-400 font-mono text-xl font-bold">19:45</span>
                    </div>
                    <div class="flex-1 border-l border-slate-700 pl-8 relative">
                        <div class="absolute -left-1.5 top-2 w-3 h-3 rounded-full bg-teal-500"></div>
                        <h3 class="text-xl font-bold text-white mb-2">クロージング & 懇親会</h3>
                        <p class="text-slate-400 text-sm">ピザとドリンクを用意しています。部署を超えた交流を深めましょう。</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="register" class="py-20 bg-slate-800/50">
        <div class="container mx-auto px-6 text-center">
            <div class="max-w-2xl mx-auto glass-card p-10 rounded-2xl border border-indigo-500/20">
                <h2 class="text-3xl font-bold mb-4 text-white">Join the Event</h2>
                <p class="text-slate-300 mb-8">
                    席に限りがありますので、お早めの登録をお願いします。<br>
                    参加登録は社内ポータル、または以下のボタンからGoogleフォームへ。
                </p>
                <a href="#" class="inline-block w-full md:w-auto px-10 py-4 bg-gradient-to-r from-indigo-600 to-teal-500 rounded-lg text-white font-bold text-lg shadow-xl hover:shadow-2xl hover:shadow-indigo-500/40 transition transform hover:scale-105">
                    今すぐ参加登録する (Google Form)
                </a>
                <p class="mt-4 text-sm text-slate-500">※ 社員アカウントでのログインが必要です</p>
            </div>
        </div>
    </section>

    <footer class="bg-slate-900 py-10 border-t border-slate-800">
        <div class="container mx-auto px-6 text-center text-slate-500 text-sm">
            <p class="mb-2">お問い合わせ: 社内AI推進委員会 (Slack: #ai-study-group)</p>
            <p>&copy; 2024 AI Study Group. internal use only.</p>
        </div>
    </footer>

</body>
</html>
