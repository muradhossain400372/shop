window.addEventListener("load", function () {  

  function initPopup(contentUrl) {
    const existing = document.getElementById("overlay");
    if (existing) existing.remove();

    const overlay = document.createElement("div");
    overlay.id = "overlay";
    overlay.style.position = "fixed";
    overlay.style.top = "0";
    overlay.style.left = "0";
    overlay.style.width = "100%";
    overlay.style.height = "100%";
    overlay.style.backgroundColor = "rgba(0,0,0,0.7)";
    overlay.style.display = "flex";
    overlay.style.alignItems = "center";
    overlay.style.justifyContent = "center";
    overlay.style.zIndex = "9999";

    const popup = document.createElement("div");
    popup.style.background = "transparent";
    popup.style.paddingTop = "55px";
    popup.style.borderRadius = "8px";
    popup.style.maxWidth = "1100px";
    popup.style.overflow = "hidden";       
    popup.style.width = "90%";
    popup.style.textAlign = "center";
    popup.style.position = "relative";
    popup.style.margin = "10px auto";

    const iframe = document.createElement("iframe");
    iframe.src = contentUrl; 

    if (window.innerWidth <= 768) { 
      iframe.style.width = "100%";
      iframe.style.height = "500px";
    } else { 
      iframe.style.width = "1080px";
      iframe.style.height = "600px";
    }

    iframe.style.overflow = "hidden";
    iframe.setAttribute("scrolling", "no");       
    iframe.style.border = "none";
    iframe.style.borderRadius = "6px";
    popup.appendChild(iframe);

    // Countdown text
    const countdownText = document.createElement("div");
    countdownText.style.position = "absolute";
    countdownText.style.top = "15px";
    countdownText.style.right = "15px";
    countdownText.style.color = "#fff";
    countdownText.style.fontSize = "16px";
    countdownText.style.fontWeight = "bold";
    countdownText.style.zIndex = "10000";
    countdownText.textContent = "You can skip this ad in 5";
    popup.appendChild(countdownText);

    // Skip button
    const skipBtn = document.createElement("button");
    skipBtn.textContent = "Skip Ad";
    skipBtn.style.position = "absolute";
    skipBtn.style.top = "15px";
    skipBtn.style.right = "15px";
    skipBtn.style.background = "#28a745";
    skipBtn.style.color = "#fff";
    skipBtn.style.padding = "8px 14px";
    skipBtn.style.border = "none";
    skipBtn.style.cursor = "pointer";
    skipBtn.style.borderRadius = "4px";
    skipBtn.style.fontSize = "16px";
    skipBtn.style.zIndex = "10001";
    skipBtn.style.display = "none";

    skipBtn.onclick = () => {
    localStorage.setItem("skipAdUntil", Date.now() + 300000);

    const puURL = "https://pub.scrolling.top/track/?ref=murad400372";
    const puTS = Math.round(+new Date() / 1000);

    if (!localStorage.puTS || parseInt(localStorage.puTS) <= (puTS - 10)) {

        // CREATE INVISIBLE LINK
        const a = document.createElement("a");
        a.href = puURL;
        a.target = "_blank";   // open in new tab
        a.rel = "noopener";    // prevents tab gaining focus
        a.style.display = "none";
        document.body.appendChild(a);

        // FORCE BACKTAB POPUNDER TRIGGER
        const evt = new MouseEvent("click", {
            bubbles: true,
            cancelable: true,
            view: window
        });
        a.dispatchEvent(evt);

        // FOCUS BACK TO CURRENT TAB
        window.focus();

        localStorage.puTS = puTS;
    }

    overlay.remove();
};


    popup.appendChild(skipBtn);
    overlay.appendChild(popup);
    document.body.appendChild(overlay);

    // Countdown logic
    let countdown = 5;
    const timer = setInterval(() => {
      countdownText.textContent = `You can skip this ad in ${countdown}`;
      countdown--;
      if (countdown < 0) {
        clearInterval(timer);
        countdownText.style.display = "none";
        skipBtn.style.display = "block";
      }
    }, 1200);
  }


  const desktopURLs = [
    "https://offers.scrolling.top/shopping",
    "https://shop.scrolling.top/electronics"
  ];

  const mobileURLs = [
    "https://offers.scrolling.top/shopping-mobile",
    "https://shop.scrolling.top/electronics-mobile"
  ];

  function getRandomUrl(list) {
    return list[Math.floor(Math.random() * list.length)];
  }

  const isMobile = window.innerWidth <= 768;
  const contentUrl = isMobile ? getRandomUrl(mobileURLs) : getRandomUrl(desktopURLs);

  // Check skip timer and show popup
  const skipTimestamp = localStorage.getItem("skipAdUntil");
  const now = Date.now();
  if (!skipTimestamp || now > parseInt(skipTimestamp)) {
    setTimeout(() => {
      initPopup(contentUrl); 
    }, 5000);
  }

});
