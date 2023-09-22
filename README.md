# Writing Good Documentation

## Step 1 - Using Codeblocks
Codeblocks in markdown makes it *very easy* for tech people to **copy, paste, share** code.
A good __Cloud Engineer__ uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replicate or research issues.

- In order to create codeblocks in markdown, you need to use three backticks (`)
- Not to be confused with single quotation (')

```
def factorial(n)
  if n <= 1
    return 1
  else
    return n * factorial(n - 1)
  end
end

puts "Enter a number to calculate its factorial:"
number = gets.chomp.to_i

result = factorial(number)
puts "The factorial of #{number} is #{result}"
```

- When you can, you should attempt to apply syntax highlighting to your codeblocks
```ruby
def factorial(n)
  if n <= 1
    return 1
  else
    return n * factorial(n - 1)
  end
end

puts "Enter a number to calculate its factorial:"
number = gets.chomp.to_i

result = factorial(number)
puts "The factorial of #{number} is #{result}"
```

![Terraform icon](https://banner2.cleanpng.com/20180529/szy/kisspng-terraform-hashicorp-microsoft-azure-infrastructure-5b0e0b6cc80963.2449977615276470848194.jpg)

<!--Resize with HTML -->
<img src="https://banner2.cleanpng.com/20180529/szy/kisspng-terraform-hashicorp-microsoft-azure-infrastructure-5b0e0b6cc80963.2449977615276470848194.jpg" width="300" height="150" alt="Altered image" />

Good Cloud Engineers use codeblocks for both Code and Errors that appear in the console.

```bash
Traceback (most recent call last):
        2: from /usr/bin/irb:23:in '<main>'
        1: from (irb):1
RuntimeError: This is a custom error message
```
Here is an example of using a codeblock for an error that appears in bash.

## Step 3 - Use Github Flavored Markdown Task Lists

Github extends Markdown to have a list where you can check off items. [<sup>[1]</sup>](#external-references)

- [x] Final Step 1
- [ ] Final Step 2
- [ ] Final Step 3

## Step 4 - Use Emojis (Optional)

Github Flavored Markdown (GFM) upports emoji shortcodes.
Here is some examples:
:cloud:

| Name | Shortcode | Emoji |
| --- | --- |  --- |
| Cloud | `:cloud:` | :cloud: |
| Thumb | `:thumbsup:` | :thumbsup: |

## Step 5 - Github Flavored Support Tables

You can use the following markdown format to create tables:

```markdown
| Name | Shortcode | Emoji |
| --- | --- |  --- |
| Cloud | `:cloud:` | :cloud: |
| Thumb | `:thumbsup:` | :thumbsup: |
```
Github extends the functionality of Markdown tables to provide more alignment and table cell formatting options. [<sup>[2]</sup>](#external-references)

- Make note of where the backtick button is located.
- It should appear above the tab key,
- but it may vary based on your keyboard layout or type.

![Photo of Terraform](assets/terrafrom.jpeg)

> **[!NOTE]**
Highlights information that users should take into account, even when skimming.

> **[!IMPORTANT]**
Crucial information necessary for users to succeed.

> **[!WARNING]**
Critical content demanding immediate user attention due to potential risks.


## External References
- [Github Flavored Markdown Spec](https://github.github.com/gfm)
- [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#quoting-text)
- [GFM - Tasks Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists) <sup>[1]</sup>
- [GTM - Emoji Cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet)
- [GFM - Tables Extensions](https://github.github.com/gfm/#tables-extension-) <sup>[2]</sup>

