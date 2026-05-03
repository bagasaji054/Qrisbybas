<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body { font-family: sans-serif; background: #000; color: #fff; text-align: center; padding: 10px; }
        canvas { max-width: 100%; height: auto; border: 1px solid #555; background: #111; }
        .box { background: #1a1a1a; padding: 15px; border-radius: 10px; max-width: 400px; margin: 15px auto; text-align: left; border: 1px solid #333; }
        input { width: 100%; padding: 12px; margin: 10px 0; background: #000; border: 1px solid #fff; color: #fff; border-radius: 5px; box-sizing: border-box; }
        .btn { background: #ce2029; color: #fff; border: none; padding: 15px; width: 100%; font-weight: bold; border-radius: 5px; cursor: pointer; }
        label { font-size: 13px; color: #aaa; }
    </style>
</head>
<body>

    <h3>BAS STORE GENERATOR</h3>
    
    <!-- Area Pratinjau -->
    <canvas id="canvas"></canvas>

    <div class="box">
        <label>1. PILIH BACKGROUND (Template Biru)</label>
        <input type="file" id="bgInp" accept="image/*">

        <label>2. PILIH QR CODE</label>
        <input type="file" id="qrInp" accept="image/*">

        <label>3. NOMINAL</label>
        <input type="number" id="nomInp" placeholder="Contoh: 6000" oninput="render()">

        <button class="btn" onclick="unduh()">DOWNLOAD HASIL</button>
    </div>

<script>
    const cvs = document.getElementById('canvas');
    const ctx = cvs.getContext('2d');
    let imgBg = new Image();
    let imgQr = new Image();

    // Default canvas
    cvs.width = 800; cvs.height = 800;
    ctx.fillText("Upload Foto Untuk Memulai", 300, 400);

    // Fungsi Upload Background
    document.getElementById('bgInp').onchange = function(e) {
        let f = e.target.files[0];
        let r = new FileReader();
        r.onload = function(ev) {
            imgBg.onload = function() {
                cvs.width = imgBg.width;
                cvs.height = imgBg.height;
                render();
            };
            imgBg.src = ev.target.result;
        };
        r.readAsDataURL(f);
    };

    // Fungsi Upload QR
    document.getElementById('qrInp').onchange = function(e) {
        let f = e.target.files[0];
        let r = new FileReader();
        r.onload = function(ev) {
            imgQr.onload = function() { render(); };
            imgQr.src = ev.target.result;
        };
        r.readAsDataURL(f);
    };

    function render() {
        if (imgBg.src) ctx.drawImage(imgBg, 0, 0);
        
        // Letak QR (Sesuai area biru)
        if (imgQr.src) ctx.drawImage(imgQr, 53, 175, 560, 560);

        // Teks Nominal (Sesuai area merah)
        let n = document.getElementById('nomInp').value;
        if (n) {
            let txt = new Intl.NumberFormat('id-ID', {
                style: 'currency', currency: 'IDR'
            }).format(n);
            
            ctx.font = "bold 42px Arial";
            ctx.fillStyle = "white";
            ctx.textAlign = "center";
            // Nilai 825 adalah koordinat Y (sudah saya turunkan)
            ctx.fillText(txt, 604, 825);
        }
    }

    function unduh() {
        let l = document.createElement('a');
        l.download = 'BAS_STORE_FIX.png';
        l.href = cvs.toDataURL();
        l.click();
    }
</script>

</body>
</html>
