# Numberic Text Box
>Make a textbox allow only numeric characters ( 0-9 , ',' ,'.' ) 

### Step 1  
  Make a textbox and add `onTextChanged` event .
### Step 2  
  ```
   private void NumericCheck(object sender, TextChangedEventArgs e)
        {
            var changes = e.Changes.Last();
            string AddedText = "";
            if (changes.AddedLength > 0)
            {
                AddedText = ((TextBox)sender).Text.Substring(changes.Offset, changes.AddedLength);
            }
            try
            {

                int.Parse(((TextBox)sender).Text.Replace(".", ",").Replace(",", ""));
            }
            catch
            {
                try
                {

                    ((TextBox)sender).Text = ((TextBox)sender).Text.Replace(AddedText, "");
                    ((TextBox)sender).Select(((TextBox)sender).Text.Length, 0);

                }
                catch
                {
                    ((TextBox)sender).Text = "";
                }
            }
        }
  ```
  You are done !
