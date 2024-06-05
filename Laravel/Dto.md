## DTO

### DTOファイルでバリデーションと変換を行うパターン
```php
final class DtoClass
{
    public readonly string $name;
    public readonly string $email;

    protected function rules(): array
    {
    }

    protected function messages(): array
    {
    }

    protected function attributes(): array
    {
    }

    public static function fromArray(): array
    {
    }

    public static function fromRequest(): array
    {
    }
}
```

#### 参考URL : [https://github.com/WendellAdriel/laravel-validated-dto/tree/main/src](https://github.com/WendellAdriel/laravel-validated-dto/tree/main/src)
