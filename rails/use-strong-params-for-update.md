# Use Strong Params To Update Record

When updating an object in rails using strong parameters in the `object_params`
method below prevents mass assignment vulnerability.

```
  def update
    @object = Object.find(params[:id])
      if @object.update(object_params)
      # handle update
  end


private
  def object_params
    params.require(:object).permit(:name, :email, :password)
  end
```
