Form-Submission
===============
1- Using jquery Ability

Using   $('#theForm')[0].reset(); or
        $('#theForm').trigger("reset");

<form id="theForm" method="" action="">
    <input type="text" class="removeLater" name="name" /> Username<br/><br />
    <input type="checkbox" class="removeLater" name="subscribe" /> Subscribe<br/><br />
    <input type="radio" class="removeLater" name="sex" value="male"> Male<br>
    <input type="radio" class="removeLater" name="sex" value="female"> Female<br/><br />
    <select>
      <option value="1">Select From The List</option>
      <option value="saab">Saab</option>
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </select><br/><br />     
    <button type="submit" class="btn-sm" id="submit">Submit</button>
    <button type="button" class="btn-sm" id="resetbtn">Reset</button>
</form>

$(function () {
    $("#resetbtn").on("click", function (e) {
        e.preventDefault();
        //$('#theForm')[0].reset();
        $('#theForm').trigger("reset");
    });
});

2- Using HTML 5 Reset Type

  <input type="reset" class="btn-sm" id="reset">
  
<form id="theForm" method="" action="">
    <input type="text" class="removeLater" name="name" /> Username<br/><br />
    <input type="checkbox" class="removeLater" name="subscribe" /> Subscribe<br/><br />
    <input type="radio" class="removeLater" name="sex" value="male"> Male<br>
    <input type="radio" class="removeLater" name="sex" value="female"> Female<br/><br />
    <select>
      <option value="1">Select From The List</option>
      <option value="saab">Saab</option>
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </select><br/><br />     
    <button type="submit" class="btn-sm" id="submit">Submit</button>
    <input type="reset" class="btn-sm" id="reset">
</form>  



URL=

http://jsfiddle.net/Behseini/t8nj2pm5/
http://jsfiddle.net/Behseini/j1xd2L4b/
