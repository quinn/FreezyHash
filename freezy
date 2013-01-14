class FreezyHash < SimpleDelegator
  def []= key, val
    if freezy.include?(key)
      puts "WARNING: cannot alter #{key}"
      return
    end

    super
  end

  def freezy val = false
    @freezy ||= []
    if val
      @freezy << val
      @freezy.uniq!
    else
      @freezy
    end
  end
end
