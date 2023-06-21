```rs
use anyhow::Result;
use rand::seq::SliceRandom;

fn main() {
    let programmer: Programmer = Programmer{
        name: "Hayden Gray",
        languages: 
            vec!["Python",
            "C", 
            "C++", 
            "Rust",
            "Dart",
            "JS/TS",
            "Terraform"
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

    fn do_work(&self) -> Result<Product> {
        let language = self.languages.choose(&mut rand::thread_rng());
        let mut done: bool = false;
        let mut product: Result<Product>;

        while !done {
            //Do Work
        }

        product
    }
}
```
