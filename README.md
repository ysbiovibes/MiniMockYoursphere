<!doctype html>
<html lang="th">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Mini Mock ชุดที่ 1 — Quiz</title>
<style>
  :root{font-family: "Segoe UI", Roboto, "Noto Sans", sans-serif}
  body{max-width:900px;margin:28px auto;padding:20px;background:#f7fafc;color:#102a43}
  h1{font-size:1.6rem;margin-bottom:4px}
  p.lead{color:#334e68;margin-top:0}
  .card{background:#fff;border-radius:10px;padding:16px;margin:12px 0;box-shadow:0 6px 18px rgba(16,42,67,0.06)}
  .question{margin-bottom:10px}
  .q-title{font-weight:600}
  .choices{margin-top:8px}
  label.choice{display:block;padding:8px;border-radius:6px;border:1px solid transparent;margin:6px 0;cursor:pointer}
  input[type=radio]{margin-right:8px}
  table{border-collapse:collapse;width:100%;margin-top:8px}
  td,th{border:1px solid #ccc;padding:6px;text-align:center}
  .controls{display:flex;gap:8px;flex-wrap:wrap;margin-top:14px}
  button{padding:10px 14px;border-radius:8px;border:0;cursor:pointer}
  button.primary{background:#0b6efd;color:#fff}
  button.ghost{background:#edf2ff;border:1px solid #dbe7ff}
  .result{padding:10px;margin-top:12px;border-radius:8px}
  .correct{background:#e6ffed;border:1px solid #bdebb0}
  .incorrect{background:#fff2f2;border:1px solid #ffcccc}
  .unanswered{background:#fffbe6;border:1px solid #ffe58f}

  /* toggle เฉลยละเอียด */
  details.explain{margin-top:10px;border-top:1px dashed #d0d7de;padding-top:8px;display:none}
  details.explain.show{display:block}
  details.explain summary{cursor:pointer;font-weight:600}
  /* ✅ แก้ให้เป็นคลาส (มีจุด) */
  .explain-body{margin-top:6px;color:#334e68}
  .alert{background:#fffbe6;border:1px solid #ffe58f;color:#614700;border-radius:8px;padding:10px;margin:12px 0}
  .alert a{color:inherit;text-decoration:underline}
</style>
</head>
<body>
<h1>Mini Mock ชุดที่ 1 — Quiz By Yoursphere </h1>
<p class="lead">ตอบคำถามจากข้อสอบ 15 ข้อ YOURSPHERE เป็นเจ้าของแบบทดสอบทั้งหมดรวมถึงทรัพย์สินทางปัญญาของการทดสอบและเอกสารนี้ภายใต้กฎหมายคุ้มครองลิขสิทธิ์ฯ </p>
<p class="lead">การทำซ้ำ หรือ ดัดแปลง หรือ เผยแพร่ หรือ อ้างถึง เนื้อหา และ/หรือ สารสนเทศใดๆ ทั้งหมด หรือ ส่วนหนึ่งส่วนใด ในเอกสารนี้ โดยมิได้รับอนุญาต จะถูกดำเนินคดีตามกฎหมาย </p>
<form id="quizForm">

<!-- ข้อ 1 -->
<div class="card question" data-q="1">
  <div class="q-title">1. จากสายใยอาหารข้างต้น ข้อใดไม่ถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q1" value="1">1) หากจำนวนงูลดลง เหยี่ยวจะมีจำนวนลดลงตาม แต่หนูจะมีจำนวนมากขึ้น</label>
    <label class="choice"><input type="radio" name="q1" value="2">2) ปริมาณสารพิษจะสะสมที่สิงโตมากที่สุด</label>
    <label class="choice"><input type="radio" name="q1" value="3">3) ผู้บริโภคที่มีลำดับสูงที่สุด คือสิงโต ผู้บริโภคลำดับที่ 5</label>
    <label class="choice"><input type="radio" name="q1" value="4">4) กฎ 10 เปอร์เซ็นต์ (Ten percent law) ไม่สามารถใช้ได้เพราะสายใยอาหาร มีความซับซ้อนกว่าห่วงโซ่อาหาร</label>
    <label class="choice"><input type="radio" name="q1" value="5">5) มีข้อที่ผิดมากกว่าหนึ่งข้อ</label>
  </div>
</div>

<!-- ข้อ 2 -->
<div class="card question" data-q="2">
  <div class="q-title">2. พิจารณาแผนภูมิ BOD แหล่งน้ำ ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q2" value="1">1) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ d เนื่องจากมีค่า BOD มากที่สุด บ่ง บอกถึงปริมาณจุลินทรีย์ที่มีชีวิตในแหล่งน้ำนั้น ๆ</label>
    <label class="choice"><input type="radio" name="q2" value="2">2) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ สามารถเลือกน้ำจากแหล่งน้ำ b c d หรือ e ก็ได้ เนื่องจาก มีค่า BOD ที่ค่อนข้างสูง บ่งบอกถึงปริมาณออกซิเจนที่ละลายอยู่ในน้ำ</label>
    <label class="choice"><input type="radio" name="q2" value="3">3) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ a เนื่องจากมีค่า BOD ต่ำที่สุด บ่งบอกถึงปริมาณออกซิเจนที่จุลินทรีย์ต้องใช้เพื่อย่อยสลายสารอินทรีย์</label>
    <label class="choice"><input type="radio" name="q2" value="4">4) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ a เนื่องจากมีค่า BOD ต่ำที่สุด บ่งบอกถึงปริมาณจุลินทรีย์มีชีวิตที่ต่ำ ซึ่งใช้ออกซิเจนในการหายใจต่ำลงด้วย</label>
    <label class="choice"><input type="radio" name="q2" value="5">5) สามารถใช้น้ำจากแหล่งน้ำใดก็ได้ ค่า BOD ไม่ได้บ่งบอกถึงคุณภาพน้ำโดยตรง ต้องอาศัยค่า OD ในการพิจารณาร่วมด้วย</label>
  </div>
</div>

<!-- ข้อ 3: ตารางสิ่งมีชีวิต (เดิม) -->
<div class="card question" data-q="3">
  <div class="q-title">3. ข้อใดระบุสิ่งมีชีวิตได้ถูกต้องทั้งหมด</div>
  <table>
    <tr><th>B</th><th>D</th><th>E</th><th>F</th><th>G</th></tr>
    <tr><td>ปลิงน้ำจืด</td><td>ปลาฉลาม</td><td>ไส้เดือน</td><td>ผึ้ง</td><td>หอยมือเสือ</td></tr>
    <tr><td>พยาธิแส้ม้า</td><td>เพรียงหัวหอม</td><td>ทากดูดเลือด</td><td>หมึก</td><td>พลานาเรีย</td></tr>
    <tr><td>พยาธิไส้เดือน</td><td>เม่นทะเล</td><td>ผีเสื้อ</td><td>ไส้เดือน</td><td>หอยปากเป็ด</td></tr>
    <tr><td>ไส้เดือน</td><td>ดาวทะเล</td><td>จิงโจ้น้ำ</td><td>แมลงสาบ</td><td>พยาธิใบไม้</td></tr>
    <tr><td>ไส้เดือนฝอย</td><td>ปลิงทะเล</td><td>แมงมุม</td><td>แม่เพรียง</td><td>หมึก</td></tr>
  </table>
  <div class="choices">
    <label class="choice"><input type="radio" name="q3" value="1">1</label>
    <label class="choice"><input type="radio" name="q3" value="2">2</label>
    <label class="choice"><input type="radio" name="q3" value="3">3</label>
    <label class="choice"><input type="radio" name="q3" value="4">4</label>
    <label class="choice"><input type="radio" name="q3" value="5">5</label>
  </div>
</div>

<!-- ข้อ 4 -->
<div class="card question" data-q="4">
  <div class="q-title">4. พิจารณาภาพปฏิกิริยา (E คือเอนไซม์) ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q4" value="1">1) ก และ ค</label>
    <label class="choice"><input type="radio" name="q4" value="2">2) ก และ ง</label>
    <label class="choice"><input type="radio" name="q4" value="3">3) ข และ ค</label>
    <label class="choice"><input type="radio" name="q4" value="4">4) ข และ ง</label>
    <label class="choice"><input type="radio" name="q4" value="5">5) ค และ ง</label>
  </div>
</div>

<!-- ข้อ 5 -->
<div class="card question" data-q="5">
  <div class="q-title">5. สารชีวโมเลกุล ข้อใด “ไม่ถูกต้อง”</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q5" value="1">1) ก และ ข</label>
    <label class="choice"><input type="radio" name="q5" value="2">2) ก และ ค</label>
    <label class="choice"><input type="radio" name="q5" value="3">3) ก และ ง</label>
    <label class="choice"><input type="radio" name="q5" value="4">4) ข และ ค</label>
    <label class="choice"><input type="radio" name="q5" value="5">5) ข และ ง</label>
  </div>
</div>

<!-- ข้อ 6 -->
<div class="card question" data-q="6">
  <div class="q-title">6. การหยดสารละลาย A/B กับสาหร่ายหางกระรอก ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q6" value="1">1) ก และ ข</label>
    <label class="choice"><input type="radio" name="q6" value="2">2) ก และ ค</label>
    <label class="choice"><input type="radio" name="q6" value="3">3) ก และ ง</label>
    <label class="choice"><input type="radio" name="q6" value="4">4) มีข้อถูกเพียงข้อเดียว</label>
    <label class="choice"><input type="radio" name="q6" value="5">5) ไม่มีข้อใดถูก</label>
  </div>
</div>

<!-- ข้อ 7 -->
<div class="card question" data-q="7">
  <div class="q-title">7. เคสไต/ปัสสาวะจาก ER ข้อใดถูกต้องที่สุด</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q7" value="1">1) เบาหวานชนิด 2 เพราะน้ำตาลสูง</label>
    <label class="choice"><input type="radio" name="q7" value="2">2) โปรตีนรีนัลเวนต่ำผิดปกติจากโกลเมอรูลัส</label>
    <label class="choice"><input type="radio" name="q7" value="3">3) ท่อหน่วยไตต้นผิดปกติ เพราะโปรตีนกรองสูง</label>
    <label class="choice"><input type="radio" name="q7" value="4">4) ADH จากต่อมใต้สมองหลังมาก → Na⁺ สูง</label>
    <label class="choice"><input type="radio" name="q7" value="5">5) รีแนลอาร์เทอรี่ออสโมติกสูง กระตุ้น ADH</label>
  </div>
</div>

<!-- ข้อ 8: ต่อม–ฮอร์โมน -->
<div class="card question" data-q="8">
  <div class="q-title">8. ข้อใดจับคู่ต่อมและฮอร์โมนได้ถูกต้อง</div>
  <table>
    <tr><th>ต่อม A</th><th>ต่อม B</th><th>ฮอร์โมน C</th><th>ฮอร์โมน D</th></tr>
    <tr><td>Thyroid</td><td>Parathyroid</td><td>Thyroxine</td><td>PTH</td></tr>
    <tr><td>Thyroid</td><td>Parathyroid</td><td>Calcitonin</td><td>PTH</td></tr>
    <tr><td>Thyroid</td><td>Parathyroid</td><td>PTH</td><td>Calcitonin</td></tr>
    <tr><td>Parathyroid</td><td>Thyroid</td><td>Calcitonin</td><td>PTH</td></tr>
    <tr><td>Parathyroid</td><td>Thyroid</td><td>PTH</td><td>Calcitonin</td></tr>
  </table>
  <div class="choices">
    <label class="choice"><input type="radio" name="q8" value="1">1</label>
    <label class="choice"><input type="radio" name="q8" value="2">2</label>
    <label class="choice"><input type="radio" name="q8" value="3">3</label>
    <label class="choice"><input type="radio" name="q8" value="4">4</label>
    <label class="choice"><input type="radio" name="q8" value="5">5</label>
  </div>
</div>

<!-- ข้อ 9 -->
<div class="card question" data-q="9">
  <div class="q-title">9. กราฟฮอร์โมนรอบเดือน: การเพิ่มของฮอร์โมน A หลังตกไข่ทำให้เกิดอะไร</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q9" value="1">1) ผนังมดลูกหนาตัวรอฝังตัว</label>
    <label class="choice"><input type="radio" name="q9" value="2">2) กระตุ้นตกไข่ซ้ำในรอบเดียวกัน</label>
    <label class="choice"><input type="radio" name="q9" value="3">3) ลดการดูดกลับน้ำและ Na⁺ ที่ไต</label>
    <label class="choice"><input type="radio" name="q9" value="4">4) ฮอร์โมน A ยับยั้งฮอร์โมน B</label>
    <label class="choice"><input type="radio" name="q9" value="5">5) เพิ่มการหลั่ง LH</label>
  </div>
</div>

<!-- ข้อ 10 -->
<div class="card question" data-q="10">
  <div class="q-title">10. ข้อใด “ไม่ถูกต้อง” เกี่ยวกับพฤติกรรมของสิ่งมีชีวิต</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q10" value="1">1) ไอ/จาม = innate behavior</label>
    <label class="choice"><input type="radio" name="q10" value="2">2) แซลมอนว่ายทวนน้ำจากกลิ่น = learned</label>
    <label class="choice"><input type="radio" name="q10" value="3">3) ลูกไก่ imprinting</label>
    <label class="choice"><input type="radio" name="q10" value="4">4) นกชินหุ่นไล่กา = habituation</label>
    <label class="choice"><input type="radio" name="q10" value="5">5) ชิมแปนซีใช้ไม้เขี่ยแอปเปิล = trial & error</label>
  </div>
</div>

<!-- ข้อ 11 -->
<div class="card question" data-q="11">
  <div class="q-title">11. ภาพตัดขวางต้นข้าว: ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q11" value="1">1) ก และ ข</label>
    <label class="choice"><input type="radio" name="q11" value="2">2) ก และ ค</label>
    <label class="choice"><input type="radio" name="q11" value="3">3) ข และ ค</label>
    <label class="choice"><input type="radio" name="q11" value="4">4) ก ข และ ค</label>
    <label class="choice"><input type="radio" name="q11" value="5">5) ไม่มีข้อใดถูก</label>
  </div>
</div>

<!-- ข้อ 12 -->
<div class="card question" data-q="12">
  <div class="q-title">12. การลำเลียงระยะไกลในพืช (phloem/xylem) ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q12" value="1">1) ก และ ข</label>
    <label class="choice"><input type="radio" name="q12" value="2">2) ก และ ค</label>
    <label class="choice"><input type="radio" name="q12" value="3">3) ข และ ค</label>
    <label class="choice"><input type="radio" name="q12" value="4">4) ก ข และ ค</label>
    <label class="choice"><input type="radio" name="q12" value="5">5) ไม่มีข้อใดถูก</label>
  </div>
</div>

<!-- ข้อ 13 -->
<div class="card question" data-q="13">
  <div class="q-title">13. การทดลอง DNA/mRNA (PCR/ไฮบริไดซ์) ข้อใดถูกต้อง</div>
  <div class="choices">
    <label class="choice"><input type="radio" name="q13" value="1">1) ก ข และ ค</label>
    <label class="choice"><input type="radio" name="q13" value="2">2) ก ค และ ง</label>
    <label class="choice"><input type="radio" name="q13" value="3">3) ก ค และ จ</label>
    <label class="choice"><input type="radio" name="q13" value="4">4) ก ข และ ง</label>
    <label class="choice"><input type="radio" name="q13" value="5">5) ข ค และ จ</label>
  </div>
</div>

<!-- ข้อ 14 -->
<div class="card question" data-q="14">
  <div class="q-title">14. พงศาวลีของครอบครัว — ใช่/ไม่ใช่</div>
  <div class="choices">
    <div>14.1 ความผิดปกตินี้น่าจะถ่ายทอดแบบเด่น</div>
    <label class="choice"><input type="radio" name="q14_1" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q14_1" value="no">ไม่ใช่</label>
    <div>14.2 รูปแบบการถ่ายทอดมียีนอยู่บนโครโมโซม X</div>
    <label class="choice"><input type="radio" name="q14_2" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q14_2" value="no">ไม่ใช่</label>
    <div>14.3 หาก II-4 แต่งงานกับชายที่มีความผิดปกติ ลูกทั้งหมดจะปกติ</div>
    <label class="choice"><input type="radio" name="q14_3" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q14_3" value="no">ไม่ใช่</label>
  </div>
</div>

<!-- ข้อ 15 -->
<div class="card question" data-q="15">
  <div class="q-title">15. กรณีลีเมอร์ — ใช่/ไม่ใช่</div>
  <div class="choices">
    <div>15.1 ความถี่แอลลีน A=0.6, a=0.4 จะไม่เปลี่ยนภายใต้ H-W</div>
    <label class="choice"><input type="radio" name="q15_1" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q15_1" value="no">ไม่ใช่</label>
    <div>15.2 หากกลับมาอยู่ด้วยกันจะสืบพันธุ์ได้</div>
    <label class="choice"><input type="radio" name="q15_2" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q15_2" value="no">ไม่ใช่</label>
    <div>15.3 การขาดแคลนอาหารทำให้ตายมาก เป็นการคัดเลือกโดยธรรมชาติ</div>
    <label class="choice"><input type="radio" name="q15_3" value="yes">ใช่</label>
    <label class="choice"><input type="radio" name="q15_3" value="no">ไม่ใช่</label>
  </div>
</div>

<div class="controls">
  <button type="button" class="primary" id="submitBtn">ส่งคำตอบ</button>
  <button type="button" class="ghost" id="resetBtn">ล้างคำตอบ</button>
</div>
<div id="resultArea"></div>
</form>

<script>
// ===== เฉลยตามที่กำหนด =====
const answers = {
  q1:'5', q2:'3', q3:'5', q4:'5', q5:'3', q6:'4', q7:'2', q8:'5',
  q9:'1', q10:'5', q11:'2', q12:'2', q13:'3',
  q14_1:'no', q14_2:'no', q14_3:'yes',
  q15_1:'yes', q15_2:'no', q15_3:'no'
};

// ===== เฉลยละเอียด (ถ้อยคำตามที่คุณส่งมา) =====
const explanations = {
  q1: [
    'เฉลย 5 ผิดข้อ 3 และข้อ 4 เพราะ',
    'ข้อ 3 ผิดสิ่งโต มี trophic level 5 แต่เป็นผู้บริโภคลำดับที่ 4',
    'ข้อ 4 ผิดตรงที่ กฎ 10 % ยังคงส่งผลเสมอ แค่ไม่สามารถเขียนพลังงานแจกแจงออกมาแบบห่วงโซ่ได้'
  ].join('\n'),
  q2: [
    'เฉลย 3 ตรงตามนิยาม BOD หรือ Biochemical Oxygen Demand',
    'คือปริมาณออกซิเจนที่จุลินทรีย์ต้องใช้ในการย่อยสลายสารอินทรีย์',
    'ยิ่ง BOD สูง = น้ำเน่าเสียมาก / ยิ่งต่ำ = คุณภาพดีกว่า',
    'ตัวเลือกอื่นผิดเพราะไม่ตรงนิยาม'
  ].join('\n'),
  q3: [
    'เริ่มพิจารณาจากสัตว์ที่มีเนื้อเยื้อ 3 ชั้น และมีเอ็มบริโอ → ตัด Porifera/Cnidaria',
    'แปลงรหัสจากไดโคโทมัสคีย์:',
    'A = ทางเดินอาหารไม่สมบูรณ์ → Platyhelminthes (พลานาเรีย/พยาธิใบไม้/พยาธิแส้ม้า ฯลฯ)',
    'B = ช่องลำตัวเทียม → Nematoda (ไส้เดือนฝอย/พยาธิไส้เดือน)',
    'C = dorsal nerve cord → Chordata (ปลาฉลาม, ปลา ฯลฯ)',
    'D = Deuterostome (ไม่ใช่ chordates) → Echinodermata (ดาวทะเล/เม่นทะเล)',
    'E = ecdysis → Arthropoda (ผีเสื้อ/ผึ้ง/แมลงสาบ/แมงมุม ฯลฯ)',
    'F = segmented และไม่ลอกคราบ → Annelida (ไส้เดือน/ปลิง)',
    'G = non-segmented protostome coelomates → Mollusca (หอย, หมึก ฯลฯ)',
    'ข้อควรระวัง:',
    '• ทาก/หอยทาก/ปลิงทะเล = Mollusca',
    '• ทากดูดเลือด/ปลิงบก/ปลิงน้ำจืด = Annelida',
    '• แม่เพรียง/ไส้เดือนดิน = Annelida',
    '• ไส้เดือนฝอย/พยาธิไส้เดือน = Nematoda',
    '• เพรียงหิน/เพรียงคอห่าน = Arthropoda (เพรียงอื่น ๆ บางชนิดเป็น Chordata ได้)',
    'ดังนั้นตอบ 5.'
  ].join('\n'),
  q4: [
    'เฉลย: 5. ค. และ ง. เท่านั้น',
    'ก. ผิด: substrate-level phosphorylation ต้อง “ย้ายหมู่ฟอสเฟต” ให้ ADP ได้ ATP (ในโจทย์กลับทิศ)',
    'ข. ผิด: สาร B มีขั้วมากกว่าสาร A (มีหมู่ฟอสเฟตมากกว่า 1)',
    'ค. ถูก: สารมีขั้วมากกว่า → ละลายน้ำดีกว่า (like dissolves like)',
    'ง. ถูก: competitive inhibitor แย่งจับกับ substrate → ต้องเพิ่ม [substrate] (เพิ่ม [product] ไม่ช่วย) และปฏิกิริยานี้เป็นทางเดียว ไม่ใช่ reversible'
  ].join('\n'),
  q5: [
    'เฉลย: 3. ก. และ ง. เท่านั้น',
    'ก. ผิด: ไตรกลีเซอไรด์ 1 โมเลกุล ได้ “น้ำ 3 โมเลกุล” จากการควบแน่น',
    'ข. ถูก: -OH ล่าง = α-glucose (trans), -OH บน = β-glucose (cis)',
    'ค. ถูก: Hemoglobin = 4 สาย (α2β2) → โครงสร้างจตุรภูมิ',
    'ง. ผิด: DNA/RNA ต่างกันที่ “น้ำตาล+ชนิดเบส”; ตำแหน่งจับหมู่ฟอสเฟตกับน้ำตาลเหมือนกันคือ C5’ ทั้งคู่'
  ].join('\n'),
  q6: [
    'เฉลย: 4. มีข้อที่กล่าวถูกต้องเพียงข้อเดียว',
    'ผลทดลอง: A isotonic (ไม่เปลี่ยน), B hypertonic (เหี่ยว)',
    'สรุปความเข้มข้น: hypertonic > isotonic > hypotonic',
    'ก. ถูก',
    'ข. ผิด: isotonic NaCl = 0.9%',
    'ค. ผิด: ถ้าจะเจือจาง A ให้ hypotonic ต้อง “น้อยกว่า A”',
    'ง. ผิด: หยดน้ำเจือจางมาก ๆ ลง A ทำให้เซลล์ “เต่ง” แต่ “ไม่แตก” เพราะเป็นเซลล์พืช',
    'ดังนั้นตอบ 4'
  ].join('\n'),
  q7: [
    'เฉลย: 2. คนไข้รายนี้อาจพบโปรตีนที่รีนัลเวนน้อยกว่าปกติ จากความผิดปกติที่โกลเมอรูลัส',
    'เหตุผลรวม:',
    '• มีโปรตีนใน filtrate และ Na+ สูง → ชี้ถึงความผิดปกติของการกรอง/ดูดกลับ',
    'วิเคราะห์ตัวเลือก:',
    '1) ผิด: สรุป T2DM ไม่ได้ ต้องพิจารณาเวลา/อาการอื่นร่วม (เช่น >90 นาทีหลังอาหาร, mg/dL ฯลฯ)',
    '2) ถูก: renal vein หลังกรองควรโปรตีนเท่าเดิม แต่พบลดลง → โปรตีนเล็ดรอดจาก glomerulus',
    '3) ผิด: filtrate คือหลัง glomerulus ก่อนท่อส่วนต้น จึงยังสรุป proximal tubule ตรง ๆ ไม่ได้',
    '4) ผิด: ADH (จาก posterior pituitary) เกี่ยวกับน้ำมากกว่า Na+ โดยตรง และข้อมูลไม่พอ',
    '5) ผิด: ADH ไม่ดูดกลับ Na+ (ควรเป็น aldosterone หากจะเกี่ยวกับ Na+)'
  ].join('\n'),
  q8: [
    'เฉลย: 5.',
    'ทวนความจำ:',
    'Thyroid (C cells) → Calcitonin: ลด Ca²⁺ ในเลือด (ดึงไปกระดูก, ลดดูดกลับที่ไต)',
    'Parathyroid → PTH: เพิ่ม Ca²⁺ (สลายกระดูก, เพิ่มดูดกลับที่ไต/ดูดซึมที่ลำไส้)',
    'ดังนั้น pairing ที่ถูกต้อง คือ (Parathyroid → PTH) และ (Thyroid → Calcitonin) → ข้อ 5'
  ].join('\n'),
  q9: [
    'เฉลย: 1. ผนังมดลูกหนาตัวเพื่อรอฝังตัว',
    'จากกราฟ: A = Progesterone (พุ่งหลังไข่ตก), B = Estrogen',
    '2) ผิด: ไม่มีตกไข่ซ้ำรอบเดียวกัน',
    '3) ผิด: Progesterone เพิ่มการดูดกลับน้ำและ Na+',
    '4) ผิด: Progesterone ไม่ได้ยับยั้ง Estrogen',
    '5) ผิด: Progesterone ลดการหลั่ง LH'
  ].join('\n'),
  q10: [
    'ข้อใด “กล่าวไม่ถูกต้อง”',
    'สรุป: 1–4 ถูก, 5 ผิด',
    '• ไอ/จาม = reflex → innate behavior (ถูก)',
    '• แซลมอนใช้กลิ่นจำถิ่นกำเนิด → learned (ถูก)',
    '• ลูกไก่ติดวัตถุแรก ๆ ที่เห็น/ได้ยิน → imprinting (ถูก)',
    '• คุ้นชินหุ่นไล่กา → habituation (ถูก)',
    '• ลิงใช้ไม้เขี่ยอาหารแบบ “คิดทันที” ไม่ใช่ trial & error → เป็น reasoning (ข้อนี้ผิด)'
  ].join('\n'),
  q11: [
    'เฉลย: 2. ก. และ ค. เท่านั้น',
    'ก. ถูก: ภาพ ก ดูเป็น phloem (อยู่นอกมัดท่อลำเลียง, เซลล์เล็ก, มีชีวิต, ชิด xylem)',
    'ข. ผิด: โครงสร้าง B เป็น air space',
    'ค. ถูก: C เป็น fiber (รอบนอกสุด, ผนังหนา, ตายแล้ว, มี lignin มาก)'
  ].join('\n'),
  q12: [
    'เฉลย: 2. ก. และ ค. เท่านั้น',
    'ก. ถูก: กระบวนการ 1 ใช้พลังงาน (active loading sucrose → น้ำ osmosis เข้า sieve tube → เพิ่ม turgor)',
    'ข. ผิด: กระบวนการ 2 เกิดจากความต่างแรงดันใน sieve tube จริง แต่การลำเลียงคือ “sucrose” ไม่ใช่กลูโคส',
    'ค. ถูก: กระบวนการ 3 น้ำออกจาก sieve tube ด้วย osmosis และน้ำตาลแพร่ออกสู่แหล่งรับ'
  ].join('\n'),
  q13: [
    'เฉลย: 3. ก. ค. และ จ.',
    'ก. ถูก: การทดลองแรกคือ PCR',
    'ข. ผิด: PCR ไม่ใช้ primase',
    'ค. ถูก: มีเบส U → ไม่ใช่ DNA (หรือผู้บันทึกอาจพิมพ์ผิด แต่โจทย์ตั้งใจให้กำกวม)',
    'ง. ผิด: การทดลองแรกยังไม่มี mRNA',
    'จ. ถูก: นับจากปลาย 5’ ย้อนมา 3’ พบ start codon (AUG) แล้วเข้ารหัสได้ 6 ตัว'
  ].join('\n'),
  q14: [
    'หลักการพิจารณา pedigree:',
    '1) เด่น/ด้อย – เด่นพบทุก generation, ด้อยอาจข้ามรุ่น → กรณีนี้เข้าข่าย “ด้อย”',
    '2) X-linked?',
    '  • X-linked dominant: ลูกชายเป็นโรค → แม่ต้องเป็นโรค, พ่อเป็นโรค → ลูกสาวต้องเป็นโรค (ขัดกับข้อมูลในโจทย์)',
    '  • X-linked recessive: ลูกสาวเป็นโรค → พ่อต้องเป็นโรค, แม่เป็นโรค → ลูกชายต้องเป็นโรค (ก็ขัดกับข้อมูล)',
    '  • Y-linked: พบเฉพาะชาย (ขัดกับข้อมูลว่าหญิงก็พบ)',
    '⇒ จึงน่าจะเป็น autosomal',
    '3) จีโนไทป์ของ II-4: หากเป็น autosomal recessive (aa = ผิดปกติ)',
    '   • II-3 เป็น aa, แล้วลูกทุกคนปกติ → II-4 เป็น AA หรือ Aa ก็ได้',
    '   • แต่แต่งงานกับชายที่ aa ลูกสามารถปกติได้ (สอดคล้องกับข้อ 14.3 “ใช่”)'
  ].join('\n'),
  q15: [
    '15.1 ใช่: ความถี่แอลลิล A=0.6, a=0.4 อยู่ภายใต้ H-W (ไม่มี selection/สุ่มผสมพันธุ์) → คงที่',
    '15.2 ไม่ใช่: แม้เคยเป็นสายพันธุ์เดียว แต่แยกปรับตัวนานจน barrier ทางสืบพันธุ์เกิดขึ้น → ไม่สืบพันธุ์กันได้',
    '15.3 ไม่ใช่: การตายจำนวนมากจากอาหารขาดแคลนใกล้กับ “bottleneck effect” มากกว่า natural selection (ไม่ใช่การคัดเลือกด้วยความสามารถเฉพาะตัว)'
  ].join('\n')
};

// ===== Helpers =====
function getFormValue(name){
  let els = document.getElementsByName(name);
  if (!els.length && !/^q/.test(name)) els = document.getElementsByName('q'+name);
  for (let i=0;i<els.length;i++) if (els[i].checked) return els[i].value;
  return null;
}
function prettyKey(key){ return key.replace(/^q/,'').replace('_','.'); }
function scrollToQuestion(key){
  const qNum = key.replace(/^q/,'').split('_')[0];
  const el = document.querySelector(`.question[data-q="${qNum}"]`);
  if (el) el.scrollIntoView({behavior:'smooth', block:'center'});
}
function ensureExplainToggle(qNum){
  const card = document.querySelector(`.question[data-q="${qNum}"]`);
  if (!card) return;
  if (card.querySelector('details.explain')) return; // เคยสร้างแล้ว
  const d = document.createElement('details');
  d.className = 'explain';
  const s = document.createElement('summary');
  s.textContent = 'เฉลยละเอียด (คลิกเพื่อเปิด)';
  const b = document.createElement('div');
  b.className = 'explain-body';
  const text = explanations['q'+qNum] || `เฉลยละเอียดข้อ ${qNum} — (พิมพ์รายละเอียด)`;
  // ✅ แปลง \n เป็น <br> ให้จัดบรรทัดสวย
  b.innerHTML = text.replace(/\n/g,'<br>');
  d.appendChild(s); d.appendChild(b);
  card.appendChild(d);
}
function showAllExplanations(){
  document.querySelectorAll('details.explain').forEach(d=>d.classList.add('show'));
}

// ===== ปลอดภัยในการแก้ "ข้อความช้อยส์" บนหน้า =====
function wrapChoiceTexts(){
  document.querySelectorAll('label.choice').forEach(lb=>{
    if (!lb.querySelector('.choice-text')){
      const span = document.createElement('span');
      const nodes = Array.from(lb.childNodes).filter(n=>n.nodeType===Node.TEXT_NODE && n.textContent.trim().length);
      const text = nodes.map(n=>n.textContent).join(' ').trim();
      nodes.forEach(n=>lb.removeChild(n));
      span.className = 'choice-text';
      span.textContent = text ? ' '+text : '';
      lb.appendChild(span);
    }
  });
}
function setChoices(qName, choicesMap){
  const inputs = document.querySelectorAll(`input[name="${qName}"]`);
  inputs.forEach(inp=>{
    const val = inp.value;
    const lb = inp.closest('label.choice');
    const span = lb.querySelector('.choice-text');
    if (choicesMap[val] && span){
      span.textContent = ' ' + choicesMap[val];
    }
  });
}
function setQuestionTitle(qNum, newTitle){
  const el = document.querySelector(`.question[data-q="${qNum}"] .q-title`);
  if (el) el.textContent = `${qNum}. ${newTitle}`;
}

// ===== Main =====
const submitBtn = document.getElementById('submitBtn');
const resetBtn  = document.getElementById('resetBtn');
const resultArea = document.getElementById('resultArea');

document.addEventListener('DOMContentLoaded', ()=>{
  wrapChoiceTexts();

  // === ตั้ง "หัวข้อคำถาม" ให้ตรงตามที่คุณส่งมา ===
  setQuestionTitle('2', 'พิจารณาข้อความต่อไปนี้ ข้อใดถูกต้อง');
  setQuestionTitle('4', 'ข้อใดถูกต้อง');
  setQuestionTitle('5', 'ข้อใดไม่ถูกต้อง');
  setQuestionTitle('6', 'ข้อใดถูกต้อง');
  setQuestionTitle('7', 'ท่านจะแสดงความคิดเห็นในข้อใดที่กล่าวถูกต้องที่สุด');
  setQuestionTitle('9', 'การเพิ่มขึ้นของระดับฮอร์โมน A หลังการตกไข่ทำให้เกิดกระบวนการใดในร่างกาย');
  setQuestionTitle('11', 'ข้อใดกล่าวถูกต้อง');
  setQuestionTitle('12', 'ข้อใดถูกต้อง');
  setQuestionTitle('13', 'ข้อใดถูกต้อง');

  // === ตั้ง "ถ้อยคำช้อยส์" ให้ตรงตามต้นฉบับ ===
  setChoices('q1', {
    "1": "1) หากจำนวนงูลดลง เหยี่ยวจะมีจำนวนลดลงตาม แต่หนูจะมีจำนวนมากขึ้น",
    "2": "2) ปริมาณสารพิษจะสะสมที่สิงโตมากที่สุด",
    "3": "3) ผู้บริโภคที่มีลำดับสูงที่สุด คือสิงโต ผู้บริโภคลำดับที่ 5",
    "4": "4) กฎ 10 เปอร์เซ็นต์ (Ten percent law) ไม่สามารถใช้ได้เพราะสายใยอาหารมีความซับซ้อนกว่าห่วงโซ่อาหาร",
    "5": "5) มีข้อที่ผิดมากกว่าหนึ่งข้อ"
  });
  setChoices('q2', {
    "1": "1) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ d เนื่องจากมีค่า BOD มากที่สุด บ่ง บอกถึงปริมาณจุลินทรีย์ที่มีชีวิตในแหล่งน้ำนั้น ๆ",
    "2": "2) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ สามารถเลือกน้ำจากแหล่งน้ำ b c d หรือ e ก็ได้ เนื่องจาก มีค่า BOD ที่ค่อนข้างสูง บ่งบอกถึงปริมาณออกซิเจนที่ละลายอยู่ในน้ำ",
    "3": "3) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ a เนื่องจากมีค่า BOD ต่ำที่สุด บ่งบอกถึงปริมาณออกซิเจนที่จุลินทรีย์ต้องใช้เพื่อย่อยสลายสารอินทรีย์",
    "4": "4) หากต้องการเลือกน้ำจากแหล่งน้ำมาใช้ ควรเลือกน้ำจากแหล่งน้ำ a เนื่องจากมีค่า BOD ต่ำที่สุด บ่งบอกถึงปริมาณจุลินทรีย์มีชีวิตที่ต่ำ ซึ่งใช้ออกซิเจนในการหายใจต่ำลงด้วย",
    "5": "5) สามารถใช้น้ำจากแหล่งน้ำใดก็ได้ ค่า BOD ไม่ได้บ่งบอกถึงคุณภาพน้ำโดยตรง ต้องอาศัยค่า OD ในการพิจารณาร่วมด้วย"
  });
  // ข้อ 3 เป็นเลข 1..5 อยู่แล้ว (ตาราง) ไม่ต้องแก้ข้อความช้อยส์

  setChoices('q4', {
    "1": "1) ก. และ ค. เท่านั้น",
    "2": "2) ก. และ ง. เท่านั้น",
    "3": "3) ข. และ ค. เท่านั้น",
    "4": "4) ข. และ ง. เท่านั้น",
    "5": "5) ค. และ ง. เท่านั้น"
  });

  setChoices('q5', {
    "1": "1) ก. และ ข. เท่านั้น",
    "2": "2) ก. และ ค. เท่านั้น",
    "3": "3) ก. และ ง. เท่านั้น",
    "4": "4) ข. และ ค. เท่านั้น",
    "5": "5) ข. และ ง. เท่านั้น"
  });

  setChoices('q6', {
    "1": "1) ก. และ ข. เท่านั้น",
    "2": "2) ก. และ ค. เท่านั้น",
    "3": "3) ก. และ ง. เท่านั้น",
    "4": "4) มีข้อที่กล่าวถูกต้องเพียงข้อเดียว",
    "5": "5) ไม่มีข้อความใดกล่าวถูกต้อง"
  });

  setChoices('q7', {
    "1": "1) คนไข้รายนี้น่าจะเป็นโรคเบาหวานชนิดที่ 2 เนื่องจากปริมาณน้ำตาลที่สูงกว่าค่าปกติ",
    "2": "2) คนไข้รายนี้อาจพบโปรตีนที่รีนัลเวนน้อยกว่าปกติ เนื่องจากความผิดปกติที่โกลเมอรูลัส",
    "3": "3) คนไข้รายนี้น่าจะมีความผิดปกติที่ท่อหน่วยไตส่วนต้น เนื่องจากยังพบโปรตีนสูงกว่าค่าปกติในของเหลวที่ผ่านการกรอง",
    "4": "4) หากการทำงานของไตปกติ อาจเป็นผลมาจากการหลั่งฮอร์โมนจากต่อมใต้สมองส่วนหลังที่มากเกินไป จนทำให้ความเข้มข้นของโซเดียมไอออนสูงขึ้น",
    "5": "5) เหตุการณ์นี้ทำให้มีแรงดันออสโมติกที่สูงที่บริเวณรีนัลอาร์เทอร์รี จึงทำให้เกิดการกระตุ้นให้หลั่ง ADH เพื่อดูดน้ำและโซเดียมกลับ"
  });

  // ข้อ 8 เป็นเลข 1..5 อยู่แล้ว (ตาราง) ไม่ต้องแก้ข้อความช้อยส์

  setChoices('q9', {
    "1": "1) ผนังมดลูกหนาตัวขึ้นเพื่อเตรียมให้ไข่ที่ปฏิสนธิแล้วมาฝังตัว",
    "2": "2) การตกไข่จะถูกกระตุ้นให้เกิดขึ้นซ้ำในรอบเดือนเดียวกันหากไม่มีการปฏิสนธิ",
    "3": "3) ลดการดูดกลับน้ำ และ Na+ ที่ไต",
    "4": "4) ฮอร์โมน A จะยับยั้งการเพิ่มขึ้นของฮอร์โมน B",
    "5": "5) เพิ่มการหลั่ง LH ในร่างกาย"
  });

  setChoices('q10', {
    "1": "1) พฤติกรรมการไอ/จามเมื่อมีสิ่งแปลกปลอมเข้าไปในทางเดินหายใจ จัดเป็นพฤติกรรมที่อยู่ในกลุ่ม พฤติกรรมที่มีมาตั้งแต่กำเนิด (innate behavior)",
    "2": "2) พฤติกรรมการว่ายทวนน้ำของปลาแซลมอนเพื่อกลับไปวางไข่ในแม่น้ำที่เกิดโดยอาศัยกลิ่นของแม่น้ำเป็นสิ่งเร้า จัดเป็นพฤติกรรมที่อยู่ในกลุ่ม พฤติกรรมการเรียนรู้ (learned behavior)",
    "3": "3) การเดินตามวัตถุที่ส่งเสียงและเคลื่อนที่ได้ของลูกไก่ เป็นพฤติกรรมการฝังใจ(imprinting)",
    "4": "4) การลดของอัตราการบินหนีหุ่นไล่กาของนกเกิดจากพฤติกรรมความเคยชิน (habituation)",
    "5": "5) ลิงซิมแปนซีใช้ไม้เขี่ยแอปเปิลที่วางอยู่นอกกรงและหยิบไม่ถึงเป็นพฤติกรรมการลองผิดลองถูก(trial and error)"
  });

  setChoices('q11', {
    "1": "1) ก. และ ข. เท่านั้น",
    "2": "2) ก. และ ค. เท่านั้น",
    "3": "3) ข. และ ค. เท่านั้น",
    "4": "4) ก. ข. และ ค.",
    "5": "5) ไม่มีข้อใดกล่าวถูกต้อง"
  });

  setChoices('q12', {
    "1": "1) ก. และ ข. เท่านั้น",
    "2": "2) ก. และ ค. เท่านั้น",
    "3": "3) ข. และ ค. เท่านั้น",
    "4": "ทั้ง 4. ก. ข. และ ค.",
    "5": "5) ไม่มีข้อใดกล่าวถูกต้อง"
  });

  setChoices('q13', {
    "1": "1) ก. ข. และ ค.",
    "2": "2) ก. ค. และ ง.",
    "3": "3) ก. ค. และ จ.",
    "4": "4) ก. ข. และ ง.",
    "5": "5) ข. ค. และ จ."
  });
});

submitBtn.addEventListener('click',()=>{
  // ตรวจว่าตอบครบไหม
  const keys = Object.keys(answers);
  const unanswered = keys.filter(k => getFormValue(k) == null);
  if (unanswered.length){
    const niceList = unanswered.map(prettyKey);
    resultArea.innerHTML = `
      <div class="alert">
        คุณยังตอบไม่ครบจ้า ✋ กรุณาตอบให้ครบก่อนส่ง<br>
        เว้นไว้: ${niceList.join(', ')}
      </div>`;
    scrollToQuestion(unanswered[0]);
    return;
  }

  // ตรวจคำตอบ + สรุป
  let correct=0,total=keys.length, output='';
  for(const key of keys){
    const val = getFormValue(key);
    const isCorrect = val === answers[key];
    if (isCorrect) correct++;
    const niceKey = prettyKey(key);
    const cls = isCorrect ? 'correct' : 'incorrect';
    output += `<div class='${cls}'>
      ${niceKey}: คุณตอบ ${val} — คำตอบที่ถูกคือ ${answers[key]}
    </div>`;
  }
  resultArea.innerHTML =
    `<div class='card'>ถูก ${correct} จาก ${total} (${Math.round(correct/total*100)}%) 
      <div style="margin-top:6px;">
        <button type="button" id="toggleAll" class="ghost" style="padding:6px 10px;border-radius:6px;">แสดง/ซ่อน เฉลยละเอียดทั้งหมด</button>
      </div>
    </div>` + output;

  // toggle เฉลยละเอียด
  const questionCards = new Set(
    keys.map(k => k.replace(/^q/,'').split('_')[0])
  );
  questionCards.forEach(qNum => ensureExplainToggle(qNum));
  showAllExplanations();

  const btn = document.getElementById('toggleAll');
  if (btn){
    let shown = true;
    btn.addEventListener('click',()=>{
      shown = !shown;
      document.querySelectorAll('details.explain').forEach(d=>{
        if (shown) d.classList.add('show'); else d.classList.remove('show');
      });
    });
  }
});

resetBtn.addEventListener('click',()=>{
  document.getElementById('quizForm').reset();
  resultArea.innerHTML='';
  document.querySelectorAll('details.explain').forEach(d=>d.classList.remove('show'));
});
</script>
</body>
</html>
