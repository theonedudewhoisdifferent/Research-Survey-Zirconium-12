<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Social Media Addiction & Academic Performance Survey</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: Arial, sans-serif; background: #f5f7fa; color: #333; line-height: 1.6; padding: 20px; }
    .container { max-width: 800px; margin: 0 auto; background: white; padding: 30px; border-radius: 10px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
    h1 { color: #2E74B5; text-align: center; margin-bottom: 10px; }
    h2 { color: #2E74B5; margin: 25px 0 15px; border-bottom: 2px solid #2E74B5; padding-bottom: 5px; }
    .intro { background: #eef5fb; padding: 15px; border-radius: 6px; margin-bottom: 20px; }
    .form-group { margin-bottom: 15px; }
    label { display: block; font-weight: bold; margin-bottom: 5px; }
    input[type="text"], input[type="email"], select { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 4px; font-size: 16px; }
    .likert { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 8px; }
    .likert label { font-weight: normal; display: flex; align-items: center; gap: 5px; }
    .question { margin-bottom: 20px; padding: 12px; background: #fafafa; border-left: 4px solid #2E74B5; border-radius: 4px; }
    button { background: #2E74B5; color: white; padding: 12px 30px; border: none; border-radius: 5px; font-size: 16px; cursor: pointer; width: 100%; margin-top: 20px; }
    button:hover { background: #1F4D78; }
    .success { display: none; background: #d4edda; color: #155724; padding: 15px; border-radius: 6px; margin-top: 20px; text-align: center; }
    .admin { margin-top: 30px; text-align: center; }
    #responses { display: none; margin-top: 20px; }
    table { width: 100%; border-collapse: collapse; margin-top: 10px; font-size: 14px; }
    th, td { border: 1px solid #ddd; padding: 8px; text-align: left; }
    th { background: #2E74B5; color: white; }
  </style>
</head>
<body>
  <div class="container">
    <h1>Social Media Addiction Survey</h1>
    <div class="intro">
      <p><strong>Purpose:</strong> This survey is for the research study on the relationship between social media addiction and academic performance among Senior High School students.</p>
      <p>Please answer honestly. Your responses will be used only for research purposes.</p>
    </div>

    <form id="surveyForm">
      <h2>Participant Information</h2>
      <div class="form-group">
        <label for="fname">First Name</label>
        <input type="text" id="fname" required>
      </div>
      <div class="form-group">
        <label for="lname">Last Name</label>
        <input type="text" id="lname" required>
      </div>
      <div class="form-group">
        <label for="email">Gmail (optional)</label>
        <input type="email" id="email" placeholder="example@gmail.com">
      </div>
      <div class="form-group">
        <label for="grade">Grade</label>
        <select id="grade" required>
          <option value="">Select</option>
          <option value="11">Grade 11</option>
          <option value="12">Grade 12</option>
        </select>
      </div>
      <div class="form-group">
        <label for="section">Section</label>
        <input type="text" id="section" required placeholder="e.g., Zirconium">
      </div>
      <div class="form-group">
        <label for="sex">Sex/Gender</label>
        <select id="sex" required>
          <option value="">Select</option>
          <option value="Male">Male</option>
          <option value="Female">Female</option>
          <option value="Prefer not to say">Prefer not to say</option>
        </select>
      </div>

      <h2>Social Media Addiction Questionnaire</h2>
      <p style="margin-bottom:15px;"><em>Scale: 1 = Strongly Disagree / Very Rarely &nbsp; 2 = Disagree / Rarely &nbsp; 3 = Neutral / Sometimes &nbsp; 4 = Agree / Often &nbsp; 5 = Strongly Agree / Very Often</em></p>

      <!-- Salience -->
      <div class="question">
        <strong>1. Do I spend a lot of time on social media?</strong>
        <div class="likert">
          <label><input type="radio" name="q1" value="1" required> 1</label>
          <label><input type="radio" name="q1" value="2"> 2</label>
          <label><input type="radio" name="q1" value="3"> 3</label>
          <label><input type="radio" name="q1" value="4"> 4</label>
          <label><input type="radio" name="q1" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>2. Is social media one of the most important activities in my daily life?</strong>
        <div class="likert">
          <label><input type="radio" name="q2" value="1" required> 1</label>
          <label><input type="radio" name="q2" value="2"> 2</label>
          <label><input type="radio" name="q2" value="3"> 3</label>
          <label><input type="radio" name="q2" value="4"> 4</label>
          <label><input type="radio" name="q2" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>3. How often do I think about social media even when it is not in use?</strong>
        <div class="likert">
          <label><input type="radio" name="q3" value="1" required> 1</label>
          <label><input type="radio" name="q3" value="2"> 2</label>
          <label><input type="radio" name="q3" value="3"> 3</label>
          <label><input type="radio" name="q3" value="4"> 4</label>
          <label><input type="radio" name="q3" value="5"> 5</label>
        </div>
      </div>

      <!-- Tolerance -->
      <div class="question">
        <strong>4. I feel the urge to use social media when it is not in use.</strong>
        <div class="likert">
          <label><input type="radio" name="q4" value="1" required> 1</label>
          <label><input type="radio" name="q4" value="2"> 2</label>
          <label><input type="radio" name="q4" value="3"> 3</label>
          <label><input type="radio" name="q4" value="4"> 4</label>
          <label><input type="radio" name="q4" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>5. Do I spend increasing amounts of time on social media to satisfy myself?</strong>
        <div class="likert">
          <label><input type="radio" name="q5" value="1" required> 1</label>
          <label><input type="radio" name="q5" value="2"> 2</label>
          <label><input type="radio" name="q5" value="3"> 3</label>
          <label><input type="radio" name="q5" value="4"> 4</label>
          <label><input type="radio" name="q5" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>6. I tend to use social media longer than what I intended it to be.</strong>
        <div class="likert">
          <label><input type="radio" name="q6" value="1" required> 1</label>
          <label><input type="radio" name="q6" value="2"> 2</label>
          <label><input type="radio" name="q6" value="3"> 3</label>
          <label><input type="radio" name="q6" value="4"> 4</label>
          <label><input type="radio" name="q6" value="5"> 5</label>
        </div>
      </div>

      <!-- Mood Modification (safe items only) -->
      <div class="question">
        <strong>7. I use social media to relieve stress.</strong>
        <div class="likert">
          <label><input type="radio" name="q7" value="1" required> 1</label>
          <label><input type="radio" name="q7" value="2"> 2</label>
          <label><input type="radio" name="q7" value="3"> 3</label>
          <label><input type="radio" name="q7" value="4"> 4</label>
          <label><input type="radio" name="q7" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>8. I use social media when I am bored, depressed, anxious or stressed.</strong>
        <div class="likert">
          <label><input type="radio" name="q8" value="1" required> 1</label>
          <label><input type="radio" name="q8" value="2"> 2</label>
          <label><input type="radio" name="q8" value="3"> 3</label>
          <label><input type="radio" name="q8" value="4"> 4</label>
          <label><input type="radio" name="q8" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>9. Using social media helps me lighten academic pressure.</strong>
        <div class="likert">
          <label><input type="radio" name="q9" value="1" required> 1</label>
          <label><input type="radio" name="q9" value="2"> 2</label>
          <label><input type="radio" name="q9" value="3"> 3</label>
          <label><input type="radio" name="q9" value="4"> 4</label>
          <label><input type="radio" name="q9" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>11. Do I tend to follow what I see on social media?</strong>
        <div class="likert">
          <label><input type="radio" name="q11" value="1" required> 1</label>
          <label><input type="radio" name="q11" value="2"> 2</label>
          <label><input type="radio" name="q11" value="3"> 3</label>
          <label><input type="radio" name="q11" value="4"> 4</label>
          <label><input type="radio" name="q11" value="5"> 5</label>
        </div>
      </div>

      <!-- Conflict / Withdrawal -->
      <div class="question">
        <strong>12. I become restless, irritable or troubled when I cannot use social media.</strong>
        <div class="likert">
          <label><input type="radio" name="q12" value="1" required> 1</label>
          <label><input type="radio" name="q12" value="2"> 2</label>
          <label><input type="radio" name="q12" value="3"> 3</label>
          <label><input type="radio" name="q12" value="4"> 4</label>
          <label><input type="radio" name="q12" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>13. Has social media affected my grades negatively?</strong>
        <div class="likert">
          <label><input type="radio" name="q13" value="1" required> 1</label>
          <label><input type="radio" name="q13" value="2"> 2</label>
          <label><input type="radio" name="q13" value="3"> 3</label>
          <label><input type="radio" name="q13" value="4"> 4</label>
          <label><input type="radio" name="q13" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>14. Has social media caused mental or physical health problems lately?</strong>
        <div class="likert">
          <label><input type="radio" name="q14" value="1" required> 1</label>
          <label><input type="radio" name="q14" value="2"> 2</label>
          <label><input type="radio" name="q14" value="3"> 3</label>
          <label><input type="radio" name="q14" value="4"> 4</label>
          <label><input type="radio" name="q14" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>15. My eyes are now sensitive due to social media.</strong>
        <div class="likert">
          <label><input type="radio" name="q15" value="1" required> 1</label>
          <label><input type="radio" name="q15" value="2"> 2</label>
          <label><input type="radio" name="q15" value="3"> 3</label>
          <label><input type="radio" name="q15" value="4"> 4</label>
          <label><input type="radio" name="q15" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>16. Do I tend to grow irrational with decisions when my mind is focused on social media?</strong>
        <div class="likert">
          <label><input type="radio" name="q16" value="1" required> 1</label>
          <label><input type="radio" name="q16" value="2"> 2</label>
          <label><input type="radio" name="q16" value="3"> 3</label>
          <label><input type="radio" name="q16" value="4"> 4</label>
          <label><input type="radio" name="q16" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>17. Do I tend to lose track of time while using social media?</strong>
        <div class="likert">
          <label><input type="radio" name="q17" value="1" required> 1</label>
          <label><input type="radio" name="q17" value="2"> 2</label>
          <label><input type="radio" name="q17" value="3"> 3</label>
          <label><input type="radio" name="q17" value="4"> 4</label>
          <label><input type="radio" name="q17" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>18. I have neglected my school activities or tasks due to the time spent on social media.</strong>
        <div class="likert">
          <label><input type="radio" name="q18" value="1" required> 1</label>
          <label><input type="radio" name="q18" value="2"> 2</label>
          <label><input type="radio" name="q18" value="3"> 3</label>
          <label><input type="radio" name="q18" value="4"> 4</label>
          <label><input type="radio" name="q18" value="5"> 5</label>
        </div>
      </div>
      <div class="question">
        <strong>19. Has social media affected my sleep schedule?</strong>
        <div class="likert">
          <label><input type="radio" name="q19" value="1" required> 1</label>
          <label><input type="radio" name="q19" value="2"> 2</label>
          <label><input type="radio" name="q19" value="3"> 3</label>
          <label><input type="radio" name="q19" value="4"> 4</label>
          <label><input type="radio" name="q19" value="5"> 5</label>
        </div>
      </div>

      <h2>Additional Information</h2>
      <div class="form-group">
        <label for="platforms">What social media applications or platforms do you use often?</label>
        <input type="text" id="platforms" placeholder="e.g., TikTok, Instagram, YouTube">
      </div>
      <div class="form-group">
        <label for="hours">On average, how many hours do you spend using social media on a day-to-day basis?</label>
        <input type="text" id="hours" placeholder="e.g., 3-4 hours">
      </div>
      <div class="form-group">
        <label for="games">Do you also use video games from trending reels, videos, or any form of content from influencers?</label>
        <select id="games">
          <option value="">Select</option>
          <option value="Yes">Yes</option>
          <option value="No">No</option>
          <option value="Sometimes">Sometimes</option>
        </select>
      </div>

      <button type="submit">Submit Survey</button>
    </form>

    <div class="success" id="successMsg">
      Thank you! Your response has been recorded.
    </div>

    <div class="admin">
      <button type="button" id="viewBtn" style="width:auto; background:#555;">View All Responses (Admin)</button>
      <button type="button" id="downloadBtn" style="width:auto; background:#28a745; margin-left:10px;">Download Responses as CSV</button>
    </div>
    <div id="responses"></div>
  </div>

  <script>
    const form = document.getElementById('surveyForm');
    const successMsg = document.getElementById('successMsg');
    const responsesDiv = document.getElementById('responses');

    function getResponses() {
      return JSON.parse(localStorage.getItem('surveyResponses') || '[]');
    }

    function saveResponse(data) {
      const responses = getResponses();
      data.timestamp = new Date().toISOString();
      responses.push(data);
      localStorage.setItem('surveyResponses', JSON.stringify(responses));
    }

    form.addEventListener('submit', function(e) {
      e.preventDefault();
      const formData = new FormData(form);
      const data = {};
      formData.forEach((value, key) => data[key] = value);
      // Also capture radio values properly
      data.q1 = form.querySelector('input[name="q1"]:checked')?.value || '';
      data.q2 = form.querySelector('input[name="q2"]:checked')?.value || '';
      data.q3 = form.querySelector('input[name="q3"]:checked')?.value || '';
      data.q4 = form.querySelector('input[name="q4"]:checked')?.value || '';
      data.q5 = form.querySelector('input[name="q5"]:checked')?.value || '';
      data.q6 = form.querySelector('input[name="q6"]:checked')?.value || '';
      data.q7 = form.querySelector('input[name="q7"]:checked')?.value || '';
      data.q8 = form.querySelector('input[name="q8"]:checked')?.value || '';
      data.q9 = form.querySelector('input[name="q9"]:checked')?.value || '';
      data.q11 = form.querySelector('input[name="q11"]:checked')?.value || '';
      data.q12 = form.querySelector('input[name="q12"]:checked')?.value || '';
      data.q13 = form.querySelector('input[name="q13"]:checked')?.value || '';
      data.q14 = form.querySelector('input[name="q14"]:checked')?.value || '';
      data.q15 = form.querySelector('input[name="q15"]:checked')?.value || '';
      data.q16 = form.querySelector('input[name="q16"]:checked')?.value || '';
      data.q17 = form.querySelector('input[name="q17"]:checked')?.value || '';
      data.q18 = form.querySelector('input[name="q18"]:checked')?.value || '';
      data.q19 = form.querySelector('input[name="q19"]:checked')?.value || '';

      saveResponse(data);
      form.reset();
      successMsg.style.display = 'block';
      setTimeout(() => successMsg.style.display = 'none', 4000);
    });

    document.getElementById('viewBtn').addEventListener('click', function() {
      const responses = getResponses();
      if (responses.length === 0) {
        responsesDiv.innerHTML = '<p>No responses yet.</p>';
        responsesDiv.style.display = 'block';
        return;
      }
      let html = '<h2>Recorded Responses</h2><table><tr><th>#</th><th>Name</th><th>Grade</th><th>Section</th><th>Timestamp</th></tr>';
      responses.forEach((r, i) => {
        html += `<tr><td>${i+1}</td><td>${r.fname} ${r.lname}</td><td>${r.grade}</td><td>${r.section}</td><td>${r.timestamp || ''}</td></tr>`;
      });
      html += '</table><p style="margin-top:10px;">Total: ' + responses.length + ' responses</p>';
      responsesDiv.innerHTML = html;
      responsesDiv.style.display = 'block';
    });

    document.getElementById('downloadBtn').addEventListener('click', function() {
      const responses = getResponses();
      if (responses.length === 0) {
        alert('No responses to download.');
        return;
      }
      const headers = Object.keys(responses[0]);
      const csv = [headers.join(','), ...responses.map(r => headers.map(h => `"${(r[h] || '').toString().replace(/"/g, '""')}"`).join(','))].join('\n');
      const blob = new Blob([csv], { type: 'text/csv' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'survey_responses.csv';
      a.click();
      URL.revokeObjectURL(url);
    });
  </script>
</body>
</html>
