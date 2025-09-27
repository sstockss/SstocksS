<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>मध्यभागी असलेले कंटेंट (Centered Content)</title>
    <!-- Tailwind CSS Load करण्यासाठी स्क्रिप्ट -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* फॉन्ट सेट करणे */
        body {
            font-family: 'Inter', sans-serif;
        }

        /* Flexbox वापरून पूर्ण कंटेंट मध्यभागी आणण्यासाठी CSS */
        .full-page-center {
            /* 100vh म्हणजे संपूर्ण स्क्रीनची उंची */
            min-height: 100vh; 
            
            /* Flexbox ॲक्टिव्हेट करा */
            display: flex;
            
            /* कंटेन्ट आडव्या दिशेने (Horizontal) मध्यभागी आणा */
            justify-content: center;
            
            /* कंटेन्ट उभ्या दिशेने (Vertical) मध्यभागी आणा */
            align-items: center;
            
            /* पृष्ठभूमीचा रंग */
            background-color: #0f172a; /* slate-900 */
        }
        
        /* कंटेन्ट बॉक्सला स्टाईल देण्यासाठी */
        .content-box {
            /* जास्तीत जास्त रुंदी सेट करा */
            max-width: 90%; 
            padding: 2.5rem; /* p-10 */
            background-color: #1e293b; /* slate-800 */
            border-radius: 1rem; /* rounded-xl */
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.2);
            text-align: center;
        }
        
        /* हेडिंग आणि लिंक्सला स्टाईल देण्यासाठी */
        .content-box h1, .content-box h2 {
            margin-bottom: 0.5rem;
            color: #f8fafc; /* slate-50 */
        }
        .content-box p {
            color: #94a3b8; /* slate-400 */
            margin-bottom: 1.5rem;
        }
        .icon-link {
             /* आयकॉनला थोडी जागा आणि गडद सीमा द्या */
            margin: 0 0.5rem; 
            padding: 0.25rem;
            border-radius: 0.5rem;
            transition: transform 0.2s;
        }
        .icon-link:hover {
            transform: scale(1.1);
        }
        .social-icons img {
             /* सोशल आयकॉनला थोडी मोठी जागा द्या */
             margin: 0 0.4rem;
        }
        .stats-image {
             /* GitHub Stats इमेजला थोडी जागा द्या */
             margin: 1.5rem 0;
        }
    </style>
</head>
<body>

<!-- हा कंटेनर Flexbox वापरून सर्व कंटेंट पेजच्या मध्यभागी ठेवतो -->
<div class="full-page-center">
    
    <!-- मुख्य कंटेंट बॉक्स -->
    <div class="content-box">
        
        <!-- तुमचा पहिला भाग -->
        <h1 class="text-5xl font-extrabold text-white">SstocksS</h1>
        <p class="text-xl text-indigo-400 mb-8">www.sstockss.com</p>
        <h2 class="text-2xl font-semibold text-gray-200 mb-6">व्यापक कार्यक्षमतेसाठी विशेष तंत्रिक भाषा आणि साधनांचा वापर</h2>
        
        <!-- आयकॉन सेक्शन -->
        <p class="flex justify-center flex-wrap gap-4 mb-10">
            <!-- मूळ आयकॉन स्ट्रक्चर, फक्त अतिरिक्त `center` टॅग्ज काढले आहेत -->
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="42" height="42" />
            </a>
            <a target="_blank" href="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original-wordmark.svg" class="icon-link">
                <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original-wordmark.svg" alt="dotnet" width="42" height="42" />
            </a>
            <a target="_blank" href="https://www.vectorlogo.zone/logos/ifttt/ifttt-ar21.svg" class="icon-link">
                <img src="https://www.vectorlogo.zone/logos/ifttt/ifttt-ar21.svg" alt="ifttt" width="42" height="42" />
            </a>
        </p>

        <!-- Recent Posts Section -->
        <h2 class="text-xl font-semibold text-gray-200 border-t pt-6 border-gray-700 mt-6">✒️ Recent Posts</h2>
        <ul class="text-left list-disc list-inside text-blue-300 mx-auto w-fit mt-4 mb-8">
            <li class="mb-2"><a target="_blank" href="www.bharat369.com" class="hover:text-blue-200">GitHub मध्ये लॉग इन करा: तुमच्या GitHub खात्यात (Account) यूजरनेम आणि पासवर्ड वापरून लॉग इन करा.</a></li>
        </ul>

        <!-- Where to find me Section -->
        <h2 class="text-xl font-semibold text-gray-200">⚡️ Where to find me</h2>
        <p class="social-icons flex justify-center flex-wrap mt-4 mb-6">
            <a target="_blank" href="https://x.com/@bharat" class="icon-link">
                <img src="https://img.shields.io/badge/twitter-x?style=for-the-badge&logo=x&logoColor=white&color=%230f1419" alt="twitter" />
            </a>
            <a target="_blank" href="https://www.facebook.com/bharatfb" class="icon-link">
                <img src="https://img.shields.io/badge/facebook-logo?style=for-the-badge&logo=facebook&logoColor=white&color=%230866ff" alt="facebook" />
            </a>
            <a target="_blank" href="https://www.instagram.com/bharatinstagram" class="icon-link">
                <img src="https://img.shields.io/badge/instagram-logo?style=for-the-badge&logo=instagram&logoColor=white&color=%23F35369" alt="instagram" />
            </a>
            <a target="_blank" href="https://www.youtube.com/BbharatT" class="icon-link">
                <img src="https://img.shields.io/badge/youtube-logo?style=for-the-badge&logo=youtube&logoColor=white&color=%23cc0000" alt="youtube" />
            </a>
        </p>

        <!-- GitHub Stats Images -->
        <p class="flex flex-col items-center">
            <img class="stats-image max-w-full h-auto" src="https://github-readme-stats.vercel.app/api?username=Bharat&show_icons=true&locale=en&theme=dark" alt="Bharat GitHub Stats" />
            <img class="stats-image max-w-full h-auto" src="https://github-readme-streak-stats.herokuapp.com/?user=Bharat&theme=dark" alt="Bharat GitHub Streak" />
            <img class="stats-image max-w-full h-auto" src="https://github-readme-stats.vercel.app/api/top-langs?username=Bharat&show_icons=true&locale=en&layout=compact&theme=dark" alt="Bharat Top Languages" />
            <a href="https://github.com/ryo-ma/github-profile-trophy">
                <img class="stats-image max-w-full h-auto" src="https://github-profile-trophy.vercel.app/?username=Bharat" alt="Bharat GitHub Trophies" />
            </a>
        </p>
    </div>
</div>

</body>
</html>
