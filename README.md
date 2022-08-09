```rs
use std::fmt::Error;
use rand::seq::SliceRandom;

fn main() {
    let programmer: Programmer = Programmer{
        name: "Hayden Gray",
        languages: 
            ["Python",
            "C", 
            "C++", 
            "Rust",
            "Dart",
            "JS/TS",
            ]};

    programmer.hello_world();
    programmer.do_work();
}

struct Programmer {
    name: str,
    languages: Vec<str>,
}

impl Programmer {
    fn hello_world(&self) -> String {
        format!("Hello, my name is {} ", self.name)
    }

    fn do_work(&self) -> Result<Product, Error> {
        let language = self.languages.choose(&mut rand::thread_rng());
        let mut done: bool = false;
        let mut product: Result<Product, Error>;

        while !done {
            //Do Work
        }

        return product
    }
}
```

<!---
A1029384756/A1029384756 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=A1029384756&show_icons=true&theme=gruvbox)](https://github.com/anuraghazra/github-readme-stats)
