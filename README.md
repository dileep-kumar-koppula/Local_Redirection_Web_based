# Local Search Engine

---

## Styling (CSS)

The webpage uses **flexbox** layout, which centers the content. Each website box has a logo and a name with hover animation that scales the box up slightly for better visual effect. The content is wrapped in a responsive grid system.

## External Libraries Used
- Bootstrap 5.2 (for grid layout and animations)
- Popper.js (for tooltips and popovers in Bootstrap)
- Icons (e.g., "bi bi-globe" from Bootstrap Icons)

## Notes
- The website logos are placed within `div` elements with a hover effect.
- The page is designed to be responsive, showing 4 items per row on medium screens, and adjusting accordingly on smaller screens.

## Website Thumbnails

- [LocalHost](http://localhost)
- [YouTube](https://www.youtube.com)
- [YahooBaba.Net](https://www.yahoobaba.net)
- [DuckDuckGo](https://www.duckduckgo.com/)
- [Blackbox AI Chat](https://www.blackbox.ai/)
- [Deep AI Chat](https://deepai.org/chat)
- [ZZZ - Code Generator](https://zzzcode.ai/code-generator)

## HTML Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Local Search Engine</title>
    <style>
        /* Inline CSS for styling */
        body {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f5f5f5;
        }

        .website-box {
            position: relative;
            width: 300px;
            height: 200px;
            margin: 10px;
            background-color: #fff;
            border: 1px solid #ccc;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin: 20px;
            transition: all 0.3s ease-in-out;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .website-box:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .website-logo {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background-color: #3498db;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            font-size: 24px;
            font-weight: bold;
            z-index: 1;
        }

        .website-name {
            position: absolute;
            bottom: 10px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 16px;
            font-weight: bold;
            color: #3498db;
            text-transform: uppercase;
        }

        .row {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
        }

        .website-box {
            flex: 0 0 25%;
        }

        /* Bootstrap for animations */
        @import url('https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css');
        .animated {
            animation-duration: 1s;
            animation-fill-mode: both;
        }

        @keyframes bounceIn {
            0% {
                transform: scale(0);
            }
            50% {
                transform: scale(1.5);
                opacity: 1;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1 class="text-center mb-5">Local Search Engine</h1>
        <div class="row row-cols-1 row-cols-md-4 g-4">

            <!-- Add website thumbnails here -->
            <a href="http://localhost" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">LocalHost</div>
            </a>
            <a href="https://www.youtube.com" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">YouTube</div>
            </a>
            <a href="https://www.yahoobaba.net" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">YahooBaba.Net</div>
            </a>
            <a href="https://www.duckduckgo.com/" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">Duckduckgo</div>
            </a>
            <a href="https://blackbox.ai/" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">Blackbox AI Chat</div>
            </a>
            <a href="https://deepai.org/chat" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">Deep AI Chat</div>
            </a>
            <a href="https://zzzcode.ai/code-generator" target="_blank" class="website-box">
                <div class="website-logo">
                    <i class="bi bi-globe"></i>
                </div>
                <div class="website-name">ZZZ - Code</div>
            </a>
            
            <!-- Add more website thumbnails as needed -->
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.5/dist/umd/popper.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.min.js"></script>
</body>
</html>
